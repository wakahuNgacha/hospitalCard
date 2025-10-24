<template>
    <div class="pageHolder">
        <HomepageMenue :menuItems="menuItems"/>
        <div class="body">
            <div class="header">
                <div class="date">
                    <UIcon name="i-mdi:calendar-today" class="size-5"/>
                    <p>{{ new Date().toLocaleDateString() }}</p>
                </div>

                <div class="profile">
                    <UIcon name="i-mdi:magnify" class="size-5"/>

                    <UIcon name="i-mdi:bell-outline" class="size-5"/>



                    <div>
                        <UIcon name="i-mdi:account-circle" class="size-5"/>                        
                        <p>Smith</p>                        
                    </div>

                </div>
                
            </div>
            <hr>
        </div>        
    </div>
</template>
<script setup>
const menuItems = [
  {
    text: 'Dashboard',
    icon: 'i-mdi:view-dashboard',
    link: '/admin'
  },
  {
    text: 'Properties',
    icon: 'i-mdi:home-city',
    link: '/adminProperties'
  },
    {
        text: 'Users',
        icon: 'i-mdi:account-group',
        link: '/adminUsers'
    },
    {
        text: 'Settings',
        icon: 'i-mdi:cog-outline',
        link: '/adminSettings'
    }
]
</script>
<style scoped>
.pageHolder {
    display: flex;
    flex-direction: row;
    width: 100%;
    height: auto;
    /* background-color: lightblue; */
}
.body {
    width: 80%;
    height: 90vh;
    margin-top: 20px;
    padding-left: 20px;
    /* background-color: lightgray; */
    border-radius: 20px;
    /* border: 1px solid var(--boder); */
}
.header{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    height: 30px;
    /* background-color: lightgreen; */
}
.date{
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 5px;
}
.profile{
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 15px;
}
.profile div{
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 5px;
}
</style>
