<script setup lang="ts">
import BarChart from "@/components/BarChart.vue";
import DropDown from "@/components/DropDown.vue";
import { onMounted } from "vue";
import { useRoute } from "vue-router";

const route = useRoute();

onMounted(() => {
  console.log(route.name);
});
</script>

<template>
  <div id="main-sect">
    <DropDown />
    <div id="set-holder">
      <div class="sect">
        <div class="users">
          <div class="user">
            <div>
              <p>Active Users</p>
              <h2>27<span>/80</span></h2>
            </div>

            <div>
              <p>Questions Answered</p>
              <h2>3,298</h2>
            </div>

            <div>
              <p>Av. Session Lenght</p>
              <h2>2m 34s</h2>
            </div>
          </div>
          <div class="user-2">
            <div>
              <p id="info">
                Starting Knowledge
                <img src="@/assets/images/Icon-info.png" alt="Info" />
              </p>
              <h2>64%</h2>
              <img src="@/assets/images/Graph.png" alt="Graph" />
            </div>

            <div>
              <p>Current Knowledge</p>
              <h2>86%</h2>
              <img src="@/assets/images/Graph.png" alt="Graph" />
            </div>

            <div>
              <p>Knowledge Gain</p>
              <h2>+34%</h2>
              <img src="@/assets/images/Graph.png" alt="Graph" />
            </div>
          </div>
        </div>
        <div class="bar">
          <div id="bar-header">
            <p>Activity</p>
            <div id="month">
              <p>Month</p>
              <img src="@/assets/images/arrow_down_icon.png" alt="" />
            </div>
          </div>
          <BarChart />
        </div>
      </div>

      <div class="sect">
        <div class="topics">
          <h3>Weakest Topics</h3>
          <div>
            <div class="sub-topics">
              <div>
                <img src="@/assets/images/Rectangle_1.png" alt="Rectangle_1" />
              </div>
              <div>
                <h4 class="header">Food Safety</h4>
                <img src="@/assets/images/Progress_1.png" alt="Progress_1" />
              </div>
              <div class="percent">
                <p>74% <span>Correct</span></p>
              </div>
            </div>
            <div class="sub-topics">
              <div>
                <img src="@/assets/images/Rectangle_2.png" alt="Rectangle_2" />
              </div>
              <div>
                <h4 class="header">Compliance Basics Procedure</h4>
                <img src="@/assets/images/Progress_2.png" alt="Progress_2" />
              </div>
              <div class="percent">
                <p>52% <span>Correct</span></p>
              </div>
            </div>
            <div class="sub-topics">
              <div>
                <img src="@/assets/images/Rectangle_3.png" alt="Rectangle_3" />
              </div>
              <div>
                <h4 class="header">Company Network</h4>
                <img src="@/assets/images/Progress_3.png" alt="Progress_3" />
              </div>
              <div class="percent">
                <p>36% <span>Correct</span></p>
              </div>
            </div>
          </div>
        </div>

        <div class="topics">
          <h3>Strongest Topics</h3>
          <div>
            <div class="sub-topics">
              <div>
                <img src="@/assets/images/Rectangle_1.png" alt="Rectangle_1" />
              </div>
              <div>
                <h4 class="header">Covid Protocols</h4>
                <img src="@/assets/images/Progress_4.png" alt="Progress_4" />
              </div>
              <div class="percent">
                <p>94% <span>Correct</span></p>
              </div>
            </div>
            <div class="sub-topics">
              <div>
                <img src="@/assets/images/Rectangle_2.png" alt="Rectangle_2" />
              </div>
              <div>
                <h4 class="header">Cyber Security Basics</h4>
                <img src="@/assets/images/Progress_4.png" alt="Progress_4" />
              </div>
              <div class="percent">
                <p>92% <span>Correct</span></p>
              </div>
            </div>
            <div class="sub-topics">
              <div>
                <img src="@/assets/images/Rectangle_3.png" alt="Rectangle_3" />
              </div>
              <div>
                <h4 class="header">Social Media Policies</h4>
                <img src="@/assets/images/Progress_4.png" alt="Progress_4" />
              </div>
              <div class="percent">
                <p>89% <span>Correct</span></p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="sect">
        <div class="topics">
          <h3>User Leaderboard</h3>
          <div class="user-topics">
            <div class="leaderboard">
              <div>
                <img src="@/assets/images/Thomas.png" alt="Thomas" />
              </div>
              <div>
                <h4 class="header">Jesse Thomas</h4>
                <span>637 Points - 98% Correct</span>
              </div>
            </div>
            <div class="direction">
              <p>1</p>
              <img src="@/assets/images/up.png" alt="Up" />
            </div>
          </div>

          <div class="user-topics">
            <div class="leaderboard">
              <div>
                <img src="@/assets/images/Thisal.png" alt="Thisal" />
              </div>
              <div>
                <h4 class="header">Thisal Mathiyazhagan</h4>
                <span>637 Points - 89% Correct</span>
              </div>
            </div>
            <div class="direction">
              <p>2</p>
              <img src="@/assets/images/Down.png" alt="Down" />
            </div>
          </div>

          <div class="user-topics">
            <div class="leaderboard">
              <div>
                <img src="@/assets/images/Helen.png" alt="Helen" />
              </div>
              <div>
                <h4 class="header">Helen Chuang</h4>
                <span>637 Points - 88% Correct</span>
              </div>
            </div>
            <div class="direction">
              <p>3</p>
              <img src="@/assets/images/up.png" alt="Up" />
            </div>
          </div>

          <div class="user-topics">
            <div class="leaderboard">
              <div>
                <img src="@/assets/images/Lura.png" alt="Lura" />
              </div>
              <div>
                <h4 class="header">Lura Silverman</h4>
                <span>637 Points - 87% Correct</span>
              </div>
            </div>
            <div class="direction">
              <p>4</p>
              <img src="@/assets/images/Down.png" alt="Down" />
            </div>
          </div>
        </div>

        <div class="topics">
          <h3>Groups Leaderboard</h3>
          <div class="user-topics">
            <div class="leaderboard">
              <div>
                <h4 class="header">Houston Facility</h4>
                <span>52 Points / User - 97% Correct</span>
              </div>
            </div>
            <div class="direction">
              <p>1</p>
              <img src="@/assets/images/up.png" alt="Up" />
            </div>
          </div>

          <div class="user-topics">
            <div class="leaderboard">
              <div>
                <h4 class="header">Test Group</h4>
                <span>52 Points / User - 95% Correct</span>
              </div>
            </div>
            <div class="direction">
              <p>2</p>
              <img src="@/assets/images/Down.png" alt="Down" />
            </div>
          </div>

          <div class="user-topics">
            <div class="leaderboard">
              <div>
                <h4 class="header">Sales Leadership</h4>
                <span>52 Points / User - 87% Correct</span>
              </div>
            </div>
            <div class="direction">
              <p>3</p>
              <img src="@/assets/images/up.png" alt="Up" />
            </div>
          </div>

          <div class="user-topics">
            <div class="leaderboard">
              <div>
                <h4 class="header">Northeast Region</h4>
                <span>52 Points / User - 75% Correct</span>
              </div>
            </div>
            <div class="direction">
              <p>4</p>
              <img src="@/assets/images/Down.png" alt="Down" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
#main-sect {
  width: 100%;
  padding: 0.5rem 0;
  position: relative;
}
#set-holder {
  width: 100%;
  margin-top: 5rem;
}

.sect {
  width: 100%;
  display: flex;
  gap: 1rem;
  margin: 0.5rem 0;
  cursor: default;
  margin-top: 1.5rem;
}
.users {
  width: 100%;
  font-weight: 500;
  border-radius: 12px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.topics {
  background-color: white;
  width: 100%;
  border-radius: 12px;
  padding: 1.5rem;
}

.topics h3 {
  color: #00000080;
  font-weight: 600;
}

.sub-topics {
  display: flex;
  justify-content: space-between;
  margin-top: 1rem;
}

.user-topics {
  display: flex;
  margin-top: 1rem;
}

.header {
  font-weight: 600;
  padding-bottom: 0.5rem;
}
.percent {
  padding-top: 1rem;
}

.percent p {
  font-size: medium;
  font-weight: 600;
}
.percent span {
  color: #00000080;
  font-weight: 600;
}

.user {
  display: flex;
  justify-content: space-between;
  gap: 1rem;
  cursor: default;
}

.user-2 {
  display: flex;
  justify-content: space-between;
  gap: 0.5rem;
  cursor: default;
}

.user div {
  background-color: white;
  width: 100%;
  height: 100%;
  border-radius: 1.25rem;
  padding: 1.5rem 1rem 4.5rem 1rem;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.user-2 div {
  background-color: white;
  width: 100%;
  height: 100%;
  border-radius: 1.25rem;
  padding: 1.5rem 1rem 2.5rem 1rem;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

p {
  font-size: small;
  text-transform: capitalize;
  margin-bottom: 2rem;
  white-space: nowrap;
}

h2 span {
  color: #00000080;
  font-size: smaller;
  font-weight: 100;
}
#info {
  display: inline-block;
  vertical-align: end;
  margin-bottom: 1.2rem;
}

#info img {
  display: inline-block;
  vertical-align: end;
}

.user-2 h2,
.user-2 img {
  margin-top: 0.6rem;
}

.bar {
  width: 100%;
  background-color: white;
  padding: 1rem;
  font-weight: 500;
  border-radius: 12px;
}

#bar-header {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 1rem;
  padding-bottom: 0.2rem;
  border-bottom: 1px solid rgba(128, 128, 128, 0.2);
}

#bar-header p {
  margin: 0;
  padding: 0.5rem 0;
}
#month p {
  margin: 0;
  padding: 0.5rem 0;
  display: inline-block;
  vertical-align: middle;
  font-weight: 600;
}

#month img {
  display: inline-block;
  vertical-align: middle;
  margin-left: 0.25rem;
}

.leaderboard {
  width: 100%;
  display: flex;
  gap: 1rem;
  margin-top: 1rem;
}

.leaderboard h4 {
  font-weight: 600;
}

.leaderboard span {
  color: #00000080;
  font-weight: 600;
}
.direction {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 0.5rem;
}

.direction p {
  margin: 0;
  font-weight: 600;
}
</style>
