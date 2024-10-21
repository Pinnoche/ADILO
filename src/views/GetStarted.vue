<template>
  <div>
    <div class="header">
      <h3>Welcome to Tesla</h3>
      <p>Follow these steps to setup your account</p>
    </div>
    <div class="container">
      <div class="progress-section">
        <div class="progress-header">
          <p>Let's get you started!</p>
          <p class="progress-count">2/5</p>
        </div>
        <div class="progress-line">
          <div class="completed-line"></div>
        </div>
        <div class="steps">
          <div class="step completed">
            <span class="material-icons checkmark">check_circle</span>
            <div class="step-info">
              <p class="step-title">Create your Profile</p>
              <p class="step-desc">Provide the required information</p>
            </div>
          </div>
          <div class="step completed">
            <span class="material-icons checkmark">check_circle</span>
            <div class="step-info">
              <p class="step-title">Verify Your Account</p>
              <p class="step-desc">
                Check your email or messages for a verification link
              </p>
            </div>
          </div>
          <div class="step">
            <span class="material-icons icon">storefront</span>
            <div class="step-info">
              <p class="step-title">Finalize Your Profile</p>
              <p class="step-desc">
                Finalize your profile by providing essential information
              </p>
            </div>
          </div>

          <div class="step">
            <span class="material-icons icon">add_circle</span>
            <div class="step-info">
              <p class="step-title">Add Products or Services</p>
              <p class="step-desc">
                Begin adding your products or services to the marketplace
              </p>
            </div>
          </div>
          <div class="step">
            <span class="material-icons icon">select_all</span>
            <div class="step-info">
              <p class="step-title">Promote Your Work</p>
              <p class="step-desc">
                Utilize promotional tools to increase visibility
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  font-family: Arial, sans-serif;
  max-width: 700px;
  margin: 0 auto 20px;
  background-color: #f7f7f7;
  border-radius: 8px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.header h3 {
  max-width: 700px;
  font-size: 24px;
  font-weight: 600;
  color: rgba(204, 21, 21, 0.895);
  margin: 0 auto 5px;
}

.header p {
  color: gray;
  font-size: 14px;
  max-width: 700px;
  margin: 0 auto 25px;
}

.progress-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 15px;
}

.progress-header p {
  margin: 0;
  padding: 20px 20px 0;
}

.progress-count {
  font-weight: bold;
  font-size: 16px;
  color: gray;
}
.progress-line {
  width: 100%;
  height: 2px;
  background-color: gray;
  padding: 0;
  margin-bottom: 15px;
}
.completed-line {
  width: 40%;
  height: 100%;
  background-color: blue;
}

.steps {
  display: flex;
  flex-direction: column;
  gap: 15px;
  padding: 0 20px 20px;
}

.step {
  display: flex;
  align-items: center;
  background-color: #fff;
  padding: 15px;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.step.completed {
  border: 1px solid blue;
}

.step .checkmark {
  font-size: 18px;
  color: blue;
  background-color: #ffffff;
  margin-right: 15px;
  padding: 5px;
  border: gray solid 1px;
  border-radius: 5px;
}

.step .icon {
  font-size: 18px;
  color: gray;
  background-color: #ffffff;
  margin-right: 15px;
  padding: 5px;
  border: gray solid 1px;
  border-radius: 5px;
}

.step-info {
  display: flex;
  flex-direction: column;
}

.step-title {
  font-weight: 600;
  color: black;
  margin-bottom: 3px;
}

.step-desc {
  font-size: 14px;
  color: gray;
}
</style>
