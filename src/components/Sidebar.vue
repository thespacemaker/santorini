<template>
  <div>
    <h2 class="text-center pt-8">Contact Us</h2>
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
