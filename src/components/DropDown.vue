<script setup lang="ts">
import { ref } from "vue";
const isTimeFrame = ref(false);
const isPeople = ref(false);
const isTopic = ref(false);
const handletimeFrame = (e: MouseEvent) => {
  e.stopPropagation();
  isPeople.value = false;
  isTopic.value = false;
  isTimeFrame.value = !isTimeFrame.value;
};

const handlePeople = (e: MouseEvent) => {
  e.stopPropagation();
  isTimeFrame.value = false;
  isTopic.value = false;
  isPeople.value = !isPeople.value;
};
const handleTopic = (e: MouseEvent) => {
  e.stopPropagation();
  isPeople.value = false;
  isTimeFrame.value = false;
  isTopic.value = !isTopic.value;
};

</script>
<template>
  <div class="dropdown-section">
    <div class="card">
      <div class="frame" @click="handletimeFrame">
        <p>Timeframe: <span>All-time</span></p>
        <div>
          <img
            src="@/assets/images/arrow_down.png"
            alt="Arrow Down"
            v-if="!isTimeFrame"
          />
          <img
            src="@/assets/images/arrow_up.png"
            alt="Arrow Up"
            v-if="isTimeFrame"
          />
        </div>
      </div>
      <div class="details" v-if="isTimeFrame">
        <p>Last Month</p>
        <p>This Month</p>
        <p>This Year</p>
        <p>Custom</p>
      </div>
    </div>

    <!-- Sect 2 -->
    <div class="card">
      <div class="frame" @click="handlePeople">
        <p>People: <span>All</span></p>
        <div>
          <img
            src="@/assets/images/arrow_down.png"
            alt="Arrow Down"
            v-if="!isPeople"
          />
          <img
            src="@/assets/images/arrow_up.png"
            alt="Arrow Up"
            v-if="isPeople"
          />
        </div>
      </div>
      <div class="details" v-if="isPeople">
        <p>Last Month</p>
        <p>This Month</p>
        <p>This Year</p>
        <p>Custom</p>
      </div>
    </div>

    <!-- Sect 3 -->
    <div class="card">
      <div class="frame" @click="handleTopic">
        <p>Topic: <span>All</span></p>
        <div>
          <img
            src="@/assets/images/arrow_down.png"
            alt="Arrow Down"
            v-if="!isTopic"
          />
          <img
            src="@/assets/images/arrow_up.png"
            alt="Arrow Up"
            v-if="isTopic"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.dropdown-section {
  background-color: inherit;
  width: 100%;
  display: flex;
  justify-content: space-between;
  gap: 3%;
  position: absolute;
}

.card {
  background-color: white;
  width: 100%;
  height: 100%;
  padding: 14px 16px;
  border-radius: 20px;
  box-shadow: 0 4px 8px #0000000D;
}

.frame {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.frame span {
  font-weight: bold;
}

.details {
  padding: 8px;
  margin-top: 2px;
  border-top: 1px solid rgba(145, 144, 144, 0.256);
}

.details p {
  padding: 14px 4rem 14px 1rem;
}
.details p:hover {
  background-color: #1b59f81a;
  border-radius: 8px;
  cursor: pointer;
  color: #1b59f8;
}
</style>
