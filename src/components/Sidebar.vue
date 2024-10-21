<script setup lang="ts"></script>

<template>
  <div class="side-bar">
    <div>
      <img src="@/assets/images/tesla.png" alt="TESLA" />
    </div>
    <div class="menus">
      <ul>
        <RouterLink to="/" exact-active-class="active-link">
          <li>
            <img src="@/assets/images/flash.png" alt="Flash" />
            Reports
          </li>
        </RouterLink>
        <RouterLink to="/about" exact-active-class="active-link">
          <li>
            <img src="@/assets/images/library.png" alt="Flash" />
            Library
          </li>
        </RouterLink>
        <RouterLink to="/about" exact-active-class="active-link">
          <li>
            <img src="@/assets/images/people.png" alt="Flash" />
            People
          </li>
        </RouterLink>
        <RouterLink to="/about" exact-active-class="active-link">
          <li>
            <img src="@/assets/images/activities.png" alt="Flash" />
            Activities
          </li>
        </RouterLink>
        <p id="support">Support</p>
        <RouterLink
          to="/getstarted"
          exact-active-class="active-link"
          class="list"
        >
          <li>
            <img src="@/assets/images/bulb.png" alt="Flash" />
            Get Started
          </li>
        </RouterLink>
        <RouterLink to="/about" exact-active-class="active-link" class="list">
          <li>
            <img src="@/assets/images/settings.png" alt="Flash" />
            Settings
          </li>
        </RouterLink>
      </ul>
      <div id="profile">
        <img src="@/assets/images/profile.png" alt="Profile" />
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
  margin: 2px 0;
  border-radius: 8px;
  cursor: pointer;
  color: #1b59f8;
}

.active-link {
  li {
    background-color: #1b59f81a;
    border-radius: 8px;
    color: #1b59f8;
  }
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
  border-top: 1px solid rgba(145, 144, 144, 0.256);
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
  margin-bottom: 6px;
}

#profile p {
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
