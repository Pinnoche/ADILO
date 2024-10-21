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
                <img src="@/assets/images/icon-info.png" alt="Info" />
              </p>
              <h2>64%</h2>
              <img src="@/assets/images/graph.png" alt="Graph" />
            </div>

            <div>
              <p>Current Knowledge</p>
              <h2>86%</h2>
              <img src="@/assets/images/graph.png" alt="Graph" />
            </div>

            <div>
              <p>Knowledge Gain</p>
              <h2>+34%</h2>
              <img src="@/assets/images/graph.png" alt="Graph" />
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
                <img src="@/assets/images/rectangle_1.png" alt="Rectangle_1" />
              </div>
              <div class="progress">
                <h4 class="header">Food Safety</h4>
                <div class="weak-progress">
                  <div id="space-74"></div>
                </div>
              </div>
              <div class="percent">
                <p>74% <span>Correct</span></p>
              </div>
            </div>
            <div class="sub-topics">
              <div>
                <img src="@/assets/images/rectangle_2.png" alt="Rectangle_2" />
              </div>
              <div class="progress">
                <h4 class="header">Compliance Basics Procedure</h4>
                <div class="weak-progress">
                  <div id="space-52"></div>
                </div>
              </div>
              <div class="percent">
                <p>52% <span>Correct</span></p>
              </div>
            </div>
            <div class="sub-topics">
              <div>
                <img src="@/assets/images/rectangle_3.png" alt="Rectangle_3" />
              </div>
              <div class="progress">
                <h4 class="header">Company Network</h4>
                <div class="weak-progress">
                  <div id="space-36"></div>
                </div>
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
                <img src="@/assets/images/rectangle_1.png" alt="Rectangle_1" />
              </div>
              <div class="progress">
                <h4 class="header">Covid Protocols</h4>
                <div class="strong-progress">
                  <div id="strong-space-95"></div>
                </div>
              </div>
              <div class="percent">
                <p>95% <span>Correct</span></p>
              </div>
            </div>
            <div class="sub-topics">
              <div>
                <img src="@/assets/images/rectangle_2.png" alt="Rectangle_2" />
              </div>
              <div class="progress">
                <h4 class="header">Cyber Security Basics</h4>
                <div class="strong-progress">
                  <div id="strong-space-92"></div>
                </div>
              </div>
              <div class="percent">
                <p>92% <span>Correct</span></p>
              </div>
            </div>
            <div class="sub-topics">
              <div>
                <img src="@/assets/images/rectangle_3.png" alt="Rectangle_3" />
              </div>
              <div class="progress">
                <h4 class="header">Social Media Policies</h4>
                <div class="strong-progress">
                  <div id="strong-space-89"></div>
                </div>
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
                <img src="@/assets/images/thomas.png" alt="Thomas" />
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
                <img src="@/assets/images/thisal.png" alt="Thisal" />
              </div>
              <div>
                <h4 class="header">Thisal Mathiyazhagan</h4>
                <span>637 Points - 89% Correct</span>
              </div>
            </div>
            <div class="direction">
              <p>2</p>
              <img src="@/assets/images/down.png" alt="Down" />
            </div>
          </div>

          <div class="user-topics">
            <div class="leaderboard">
              <div>
                <img src="@/assets/images/helen.png" alt="Helen" />
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
                <img src="@/assets/images/lura.png" alt="Lura" />
              </div>
              <div>
                <h4 class="header">Lura Silverman</h4>
                <span>637 Points - 87% Correct</span>
              </div>
            </div>
            <div class="direction">
              <p>4</p>
              <img src="@/assets/images/down.png" alt="Down" />
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
              <img src="@/assets/images/down.png" alt="Down" />
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
              <img src="@/assets/images/down.png" alt="Down" />
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
  width: 100%;
  height: 48%;
  display: flex;
  justify-content: space-between;
  gap: 1rem;
  cursor: default;
}

.user-2 {
  width: 100%;
  height: 48%;
  display: flex;
  justify-content: space-between;
  gap: 0.5rem;
  cursor: default;
}

.user div {
  background-color: white;
  width: 32%;
  border-radius: 1.25rem;
  padding: 1.5rem 1rem 4.5rem 1rem;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.user-2 div {
  background-color: white;
  width: 32%;
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

.progress {
  width: 44%;
}

.weak-progress {
  width: 100%;
  height: 0.55rem;
  background-color:#ff40802d;
  border-radius: 12px;
  padding: 0;
}

#space-74 {
  width: 74%;
  height: 100%;
  background-color: #FF4080;
  border-radius: 12px;
}

#space-52 {
  width: 52%;
  height: 100%;
  background-color: #FF4080;
  border-radius: 12px;
}

#space-36 {
  width: 36%;
  height: 100%;
  background-color: #FF4080;
  border-radius: 12px;
}

.strong-progress {
  width: 100%;
  height: 0.55rem;
  background-color:#7fdd537b;
  border-radius: 12px;
  padding: 0;
}

#strong-space-95 {
  width: 94%;
  height: 100%;
  background-color: #2FEA9B;
  border-radius: 12px;
}

#strong-space-92 {
  width: 94%;
  height: 100%;
  background-color: #2FEA9B;
  border-radius: 12px;
}

#strong-space-89 {
  width: 94%;
  height: 100%;
  background-color: #2FEA9B;
  border-radius: 12px;
}
</style>
