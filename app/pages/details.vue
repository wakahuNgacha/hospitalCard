<template>
    <div class="detailsholder">
        <div class="form">
            <form action="" method="post">
                <div class="text">
                    <h3>Finish setting up your account please</h3>
                    <p>We need the information for better services</p>                    
                </div>


                <!-- Date of Birth -->
                <div class="formgroup">
                <label for="dob">Date of Birth</label>
                <input
                    type="date"
                    id="dob"
                    name="dob"
                    v-model="form.dob"
                    required
                />
                </div>

                <!-- Gender -->
                <div class="formgroup">
                <label for="gender">Gender</label>
                <select id="gender" name="gender" v-model="form.gender" required>
                    <option disabled value="">Select gender</option>
                    <option value="male">Male</option>
                    <option value="female">Female</option>
                    <option value="other">Other</option>
                </select>
                </div>

                <!-- Blood Type -->
                <div class="formgroup">
                <label for="bloodType">Blood Type</label>
                <input
                    type="text"
                    id="bloodType"
                    name="bloodType"
                    v-model="form.bloodType"
                    placeholder="e.g. O+, A-, AB+"
                    required
                />
                </div>

                <!-- Phone -->
                <div class="formgroup">
                <label for="phone">Phone</label>
                <input
                    type="tel"
                    id="phone"
                    name="phone"
                    v-model="form.phone"
                    placeholder="+254700000000"
                    required
                />
                </div>

                <!-- Emergency Contact Name -->
                <div class="formgroup">
                <label for="ecName">Emergency Contact Name</label>
                <input
                    type="text"
                    id="ecName"
                    name="ecName"
                    v-model="form.ecName"
                    placeholder="John Doe"
                    required
                />
                </div>

                <!-- Emergency Contact Phone -->
                <div class="formgroup">
                <label for="ecPhone">Emergency Contact Phone</label>
                <input
                    type="tel"
                    id="ecPhone"
                    name="ecPhone"
                    v-model="form.ecPhone"
                    placeholder="+254711111111"
                    required
                />
                </div>

                <div class="formgroup">
                    <button type="submit">Finish setting up</button>
                </div>
            </form>
        </div>
    </div>
</template>
<script setup>
const form = ref({
  dob: '',
  gender: '',
  bloodType: '',
  phone: '',
  ecName: '',
  ecPhone: ''
})

</script>
<style scoped>
.detailsholder {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    /* background-color: lightgreen; */
}
.form{
    width: 60%;
    /* background-color: tomato; */
}
.text {
    margin-bottom: 50px;
}
.formgroup {
    width: 100%;
    margin-bottom: 15px;
    display: flex;
    flex-direction: column;
}
input, select {
    width: 100%;
    padding: 10px;
    margin-top: 5px;
    border: 1px solid #ccc;
    border-radius: 5px;
    box-sizing: border-box;
}
#forgot {
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}
a {
    text-decoration: none;
    color: var(--accent);
}
</style>
