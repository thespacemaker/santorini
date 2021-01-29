<template>
  <div>
    <!-- <v-icon class="ma-4">mdi-close</v-icon> -->
    <h2 class="text-center mt-8">Contact Us</h2>
    <div class="container">
      <form method="post" action="https://formspree.io/f/xzbkonbl">
        <label for="fname">Name</label>
        <input type="text" id="fname" name="name" placeholder="Your name..">

        <label for="phone">Phone Number</label>
        <input type="text" id="lname" name="phone" placeholder="Your phone number..">

        <label for="_noReply">Email</label>
        <input type="text" id="lname" name="_noReply" placeholder="Your email..">

        <label for="subject">Message</label>
        <textarea id="subject" name="subject" placeholder="Write something.." style="height:10em;"></textarea>
        <h2 class="text-center"><input type="submit" value="Submit"></h2>
      </form>
    </div>
  </div>
</template>

<script>
  export default {}
</script>

<style scoped>
body {font-family: Arial, Helvetica, sans-serif;}
* {box-sizing: border-box;}

input[type=text], select, textarea {
  width: 100%;
  height:3em;
  background-color: #89678D;
  /* border: 1px solid #ccc; */
  border-radius: 4px;
  box-sizing: border-box;
  margin-top: 6px;
  margin-bottom: 16px;
  /* resize: vertical; */
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
  /* padding: 20px; */
}
</style>
