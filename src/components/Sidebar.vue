<script lang="ts"></script>

<template>
  <div class="side-bar">
    <div>
      <img src="@/assets/images/TESLA.png" alt="TESLA" />
    </div>
    <div class="menus">
      <ul>
        <li>
          <img src="@/assets/images/flash.png" alt="Flash" />
          Reports
        </li>
        <li>
          <img src="@/assets/images/Library.png" alt="Flash" />
          Library
        </li>
        <li>
          <img src="@/assets/images/People.png" alt="Flash" />
          People
        </li>
        <li>
          <img src="@/assets/images/Activities.png" alt="Flash" />
          Activities
        </li>
        <p id="support">Support</p>
        <li>
          <img src="@/assets/images/Bulb.png" alt="Flash" />
          Get Started
        </li>
        <li>
          <img src="@/assets/images/Settings.png" alt="Flash" />
          Settings
        </li>
      </ul>
      <div id="profile">
        <img src="@/assets/images/Profile.png" alt="Profile" />
        <h2>Sam Wheeler</h2>
        <p>ptime552@gmail.com</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.side-bar {
  width: 20%;
  padding: 1rem;
  height: 100vh;
  position: fixed;
  left: 0;
  top: 0;
  background-color: white;
  border: 2px solid white;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
}

ul {
  width: 100%;
  margin-top: 16px;
  margin-bottom: 8px;
  font-size: 14px;
}

li {
  padding: 14px 2rem;
  display: flex;
  align-items: center;
  gap: 1rem;
  white-space: nowrap;
}

li:hover {
  background-color: #1b59f81a;
  border-radius: 8px;
  cursor: pointer;
  color: #1b59f8;
}
#support {
  margin-top: 2.5rem;
  padding: 8px 16px;
  font-weight: 600;
}

.menus {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.menus div {
  padding: 2rem 16px 0;
  margin-bottom: 4rem;
  border-top: gray 1px solid;
}
.menus div h2 {
  font-size: medium;
  margin-bottom: 0.5rem;
}
.menus div p {
  font-size: small;
}
#profile {
  cursor: default;
}

#profile img {
  margin-bottom: 8px;
}

#profile p{
  color: #00000080;
  font-size: small;
}

/* @media (max-width: 768px) {
  .side-bar {
    width: 60%;
  }

  li {
    padding: 14px 1rem;
  }
}

@media (max-width: 480px) {
  .side-bar {
    width: 80%;
  }

  li {
    padding: 14px 0.5rem;
  }
} */
</style>
