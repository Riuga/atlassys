<template>
  <div class="profile">
    <nav>
      <ul>
        <li>Edit Profile</li>
        <li>Preferences</li>
        <li>Security</li>
      </ul>
    </nav>
    <img src="../assets/avatar.jpg" alt="avatar">
    <form>
      <div>
        <label for="your-name">Your Name</label>
        <input type="text" name="your-name" value="Charlene Reed">
      </div>
      <div>
        <label for="user-name">User Name</label>
        <input type="text" name="user-name" value="Charlene Reed">
      </div>
      <div>
        <label for="email">Email</label>
        <input type="email" name="email" value="charlenereed@gmail.com">
      </div>
      <div>
        <label for="password">Password</label>
        <input type="password" name="password" value="**********">
      </div>
      <div>
        <label for="date-of-birth">Date of Birth</label>
        <input type="date" name="date-of-birth" value="1990-01-25">
      </div>
      <div>
        <label for="present-address">Present Address</label>
        <input type="text" name="present-address" value="San Jose, California, USA">
      </div>
      <div>
        <label for="city">Permanent Address</label>
        <input type="text" name="permanent-address" value="San Jose, California, USA">
      </div>
      <div>
        <label for="city">City</label>
        <input type="text" name="city" value="San Jose">
      </div>
      <div>
        <label for="postal">Postal Code</label>
        <input type="text" name="postal" value="45962">
      </div>
      <div>
        <label for="country">Country</label>
        <input type="text" name="country" value="USA">
      </div>
      <button type="submit">Save</button>
    </form>
  </div>
</template>

<style lang="scss" scoped>
form {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;

  div {
    width: 50%;
    display: flex;
    flex-direction: column;
  }

  button {
    margin-left: auto;
  }
}

ul {
  display: flex;
  flex-direction: row;
  list-style-type: none;
}
</style>