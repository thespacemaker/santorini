<template>
  <div>
    <h2 class="text-center pt-8">Contact Us</h2>
    <!-- <v-form
      class="mx-8"
      ref="form"
      v-model="valid"
      lazy-validation
    >
      <v-row>
        <v-col cols="6">
          <v-text-field
            v-model="name"
            :counter="10"
            :rules="nameRules"
            label="Name"
            required
          ></v-text-field>
        </v-col>
        <v-col cols="6">
          <v-text-field
            v-model="name"
            :counter="10"
            :rules="nameRules"
            label="Name"
            required
          ></v-text-field>
        </v-col>
      </v-row>
      <v-text-field
        v-model="email"
        :rules="emailRules"
        label="E-mail"
        required
      ></v-text-field>

      <v-text-field
        v-model="name"
        :counter="10"
        :rules="nameRules"
        label="Name"
        required
      ></v-text-field>

      <v-btn
        :disabled="!valid"
        color="success"
        class="mr-4"
        @click="validate"
      >
        Validate
      </v-btn>

      <v-btn
        color="error"
        class="mr-4"
        @click="reset"
      >
        Reset Form
      </v-btn>

      <v-btn
        color="warning"
        @click="resetValidation"
      >
        Reset Validation
      </v-btn>
    </v-form> -->
    <div class="container">
      <form action="/action_page.php">
        <label for="fname">First Name</label>
        <input type="text" id="fname" name="firstname" placeholder="Your name..">

        <label for="lname">Phone Number</label>
        <input type="text" id="lname" name="lastname" placeholder="Your last name..">

        <label for="lname">Email</label>
        <input type="text" id="lname" name="lastname" placeholder="Your last name..">

        <label for="subject">Message</label>
        <textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea>
        <h2 class="text-center"><input type="submit" value="Submit"></h2>
      </form>
    </div>
  </div>
</template>

<script>
  export default {
  }
</script>

<style scoped>
body {font-family: Arial, Helvetica, sans-serif;}
* {box-sizing: border-box;}

input[type=text], select, textarea {
  width: 100%;
  padding: 12px;
  background-color: #89678D;
  /* border: 1px solid #ccc; */
  border-radius: 4px;
  box-sizing: border-box;
  margin-top: 6px;
  margin-bottom: 16px;
  resize: vertical;
}

input[type=submit] {
  background-color: #FFFFFF;
  color: black;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

input[type=submit]:hover {
  background-color: #89678D;
}

.container {
  border-radius: 5px;
  /* background-color: #f2f2f2; */
  padding: 20px;
}
</style>
