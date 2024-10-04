<template>
  <div class="profile">
    <nav>
      <ul>
        <li class="active">Edit Profile</li>
        <li>Preferences</li>
        <li>Security</li>
      </ul>
    </nav>
    <div class="content-wrapper">
      <div class="avatar-wrapper">
        <img class="avatar" src="../assets/avatar.jpg" alt="avatar">
      </div>
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
  </div>
</template>

<style lang="scss" scoped>
.profile {
  background-color: #fff;
  margin-top: 2rem;
  margin-left: 2.5rem;
  margin-right: 2.5rem;
  border-radius: 25px;
  padding: 2rem;
}

.avatar {
  border-radius: 50%;
}

.active {
  color: #1814F3;
  border-bottom: 3px solid #1814F3;
}

.content-wrapper {
  display: flex;
}

form {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;

  div {
    width: 45%;
    display: flex;
    flex-direction: column;
    margin: 30px;

  }

  input {
    border-radius: 15px;
    border: 1px solid #718EBF;
    color: #718EBF;
    padding: 1rem;
    margin-top: 10px;
  }

  button {
    margin-left: auto;
    color: white;
    background-color: #1814F3;
    font-size: 1.2rem;
    border: none;
    border-radius: 15px;
    padding: 1rem 3.5rem;
    cursor: pointer;
  }
}

ul {
  display: flex;
  flex-direction: row;
  list-style-type: none;
  color: #718EBF;
  border-bottom: 1px solid #F4F5F7;
  margin-bottom: 3rem;

  li {
    margin-right: 4rem;
    font-size: 1.3rem;
    cursor: pointer;
  }
}

@media screen and (max-width: 1770px) {
  button {
    margin-left: 0;
    width: 100%;
  }

  form {
    div {
      width: 100%;
    }
  }


}

@media screen and (max-width: 1200px) {
  li {
    span {
      display: none;
    }
  }

  .logo {
    opacity: 0;
  }
}

@media screen and (max-width: 700px) {
  .content-wrapper {
    flex-direction: column;

    .avatar-wrapper {
      margin: 0 auto;
    }
  }
}
</style>