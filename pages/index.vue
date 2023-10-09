<template>
  <div>
    <nav>
      <Navbar/>
    </nav>

    <div>
      <div class="row all-card
      ">
        <div class="profile-detile">
          <div class="top-content">
            <a><img class="link-icon" src="../static/Square Top Down.png"/></a>
            <div class="profile-dtl">
              <div class="dtl-img">
                <img class="rounded-full" src="../static/profile.png" alt="Placeholder Image">
              </div>
              <div class="dtl-contant">
                <h5>Name</h5>
                <p>IDSOS11456</p>
                <p>sandra.pv@sixtyonesteps.com</p>
              </div>
            </div>
            <div class="dtl-info">
              <div class="card-section">
                <div class="card-label">Company Name</div>
                <div class="card-value">Sixty One Steps</div>
              </div>
              <div class="card-section">
                <div class="card-label">Department & Designation</div>
                <div class="card-value">Design, Product Designer (UI/UX)</div>
              </div>
              <div class="card-section">
                <div class="card-label">Manager/Reporting to</div>
                <div class="card-value">Arun Prabhu</div>
              </div>
            </div>
          </div>
        </div>
        <div class="profile-cards col-4"><div class="container">
        <div class="circle-container">
            <div class="circle red"></div>
            <div class="circle emerald"></div>
            <div class="circle blue"></div>
        </div>
        <div class="leave-info">
            <div class="leave-label">Total Leaves</div>
            <div class="leave-count">24</div>
        </div>
        <div class="legend">
            <div class="legend-item">
                <div class="legend-dot blue"></div>
                <div class="legend-text">Pending Leave</div>
            </div>
            <div class="legend-item">
                <div class="legend-dot emerald"></div>
                <div class="legend-text">Approved Leave</div>
            </div>
            <div class="legend-item">
                <div class="legend-dot red"></div>
                <div class="legend-text">Balance Leave</div>
            </div>
        </div>
        <button class="apply-leave-button">Apply Leave</button>
    </div></div>
        <div class="profile-cards col-4">
          <div class="custom-container">
        <div class="custom-header">
            <div class="custom-header-content">
                <div class="custom-title">Pending Leave Requests</div>
                <div class="custom-filter">
                    <div class="custom-filter-label">By Date</div>
                    <div class="custom-filter-icon"></div>
                </div>
            </div>
        </div>
        <div class="custom-leave-requests">
            <div class="custom-request">
                <div class="custom-request-info">
                    <div class="custom-request-name">Name</div>
                    <div class="custom-request-date">7 October</div>
                    <div class="custom-request-reason">(Personal emergency)</div>
                </div>
                <div class="custom-delete-request">
                    <div class="custom-delete-text">Delete Request</div>
                </div>
            </div>
            <div class="custom-request">
                <div class="custom-request-info">
                    <div class="custom-request-name">Name</div>
                    <div class="custom-request-date">1 October</div>
                    <div class="custom-request-reason">(Sick)</div>
                </div>
                <div class="custom-delete-request">
                    <div class="custom-delete-text">Delete Request</div>
                </div>
            </div>
            <div class="custom-request">
                <div class="custom-request-info">
                    <div class="custom-request-name">Name</div>
                    <div class="custom-request-date">1 October</div>
                    <div class="custom-request-reason">(Casual)</div>
                </div>
                <div class="custom-delete-request">
                    <div class="custom-delete-text">Delete Request</div>
                </div>
            </div>
        </div>
        <div class="custom-vertical-line"></div>
    </div>

        </div>
        <div class="profile-cards col-4">

        </div>
        <div class="profile-cards col-4"></div>
        <div class="profile-cards col-4"></div>
        <div class="profile-cards col-4"></div>
        <div class="profile-cards col-4"></div>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: 'IndexPage'
}
</script>
<style>
/* styles.css */

.custom-container {
    width: 447px;
    height: 366px;
    background-color: #fff;
    border-radius: 15px;
    position: relative;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
}

.custom-header {
  width: 100%;
    padding: 12.5px 5px;
    background-color: #f2f2f2;
    box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.1);
    position: absolute;
    left: 0;
    top: 0;
    display: flex;
    justify-content: center;
    align-items: center;
}

.custom-header-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.custom-title {
    color: #333;
    font-size: 16px;
    font-weight: 500;
    font-family: 'Proxima Nova', sans-serif;
}

.custom-filter {
  display: flex;
    align-items: flex-end;
    gap: 2.5px;
    justify-content: center;
    flex-direction: row-reverse;
    float: right;
    flex-wrap: nowrap;
    padding-left: 145px;
}

.custom-filter-label {
    color: #555;
    font-size: 12px;
    font-weight: 500;
    font-family: 'Proxima Nova', sans-serif;
}

.custom-filter-icon {
    width: 5px;
    height: 5px;
    background-color: #ddd;
}

.custom-leave-requests {
    position: absolute;
    left: 0;
    top: 65px;
    display: flex;
    flex-direction: column;
    justify-content: start;
    align-items: start;
}

.custom-request {
    width: 437px;
    padding: 15px;
    border-bottom: 1px solid #ddd;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.custom-request-info {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: start;
    gap: 2.5px;
}

.custom-request-name {
    color: #333;
    font-size: 14px;
    font-weight: 500;
    font-family: 'Proxima Nova', sans-serif;
}

.custom-request-date {
    color: #000;
    font-size: 13px;
    font-weight: 500;
    font-family: 'Proxima Nova', sans-serif;
}

.custom-request-reason {
    color: #555;
    font-size: 11px;
    font-weight: normal;
    font-family: 'Proxima Nova', sans-serif;
}

.custom-delete-request {
    padding: 1.5px 2.5px;
    background-color: #fdd;
    border: 1px solid #fee;
    border-radius: 5px;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 2.5px;
}

.custom-delete-text {
    color: #f55;
    font-size: 13px;
    font-weight: normal;
    font-family: 'Proxima Nova', sans-serif;
}

.custom-vertical-line {
    width: 5px;
    height: 117px;
    background-color: #ddd;
    position: absolute;
    left: 442px;
    top: 127px;
    border-radius: 15px;
}

.all-card {
    width: 100%;
    padding: 0px !important;
}
.profile-detile {
    width: 447px;
    float: right;
    margin: 20px;
    background-color: white;
    box-shadow: 0 8px 70px 0 #a9a9a9;
    border-radius: 10px;
    height: 366px;
    border: solid 1px #ffbb1e;
    padding: 0px;
}
.profile-cards {
    width: 447px;
    float: right;
    margin: 20px;
    background-color: white;
    box-shadow: 0 8px 70px 0 #a9a9a9;
    border-radius: 10px;
    height: 366px;
    padding: 0px;
}
/* styles.css */

.container {
    width: 447px;
    height: 366px;
    background-color: #fff;
    border-radius: 15px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
    position: relative;
}

.circle-container {
    width: 189px;
    height: 189px;
    left: 132px;
    top: 104px;
    position: absolute;
}

.circle {
    width: 189px;
    height: 189px;
    position: absolute;
    border-radius: 50%;
}

.red {
    background-color: #FFC0CB;
}

.emerald {
    background-color: #2ecc71;
}

.blue {
    background-color: #3498db;
}

.leave-info {
    left: 25px;
    top: 35px;
    position: absolute;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
    gap: 15px;
}

.leave-label {
    color: #333;
    font-size: 16px;
    font-weight: 500;
    font-family: 'Proxima Nova', sans-serif;
}

.leave-count {
    color: #FFA500;
    font-size: 36px;
    font-weight: bold;
    font-family: 'Proxima Nova', sans-serif;
}

.legend {
    left: 25px;
    top: 326px;
    position: absolute;
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
    gap: 15px;
}

.legend-item {
    display: flex;
    align-items: center;
    gap: 5px;
}

.legend-dot {
    width: 15px;
    height: 15px;
    border-radius: 3px;
}

.blue-dot {
    background-color: #3498db;
}

.emerald-dot {
    background-color: #2ecc71;
}

.red-dot {
    background-color: #FFC0CB;
}

.apply-leave-button {
    padding: 10px 20px;
    left: 315px;
    top: 35px;
    position: absolute;
    background-color: #FFA500;
    border: none;
    border-radius: 5px;
    color: #fff;
    font-size: 14px;
    font-weight: 500;
    font-family: 'Proxima Nova', sans-serif;
    cursor: pointer;
}

@media screen and (max-width: 768px) {
.profile-detile {
    width: 334px;
    float: right;
    margin: 20px;
    background-color: white;
    box-shadow: 0 8px 70px 0 #a9a9a9;
    border-radius: 10px;
    height: 366px;
    border: solid 1px #ffbb1e;
    padding: 0px;
}
.container {
    width: 334px;
    height: 366px;
    background-color: #fff;
    border-radius: 15px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
    position: relative;
}
.all-card {
    width: 100%;
    /* padding: 54px; */
    margin: 0px;
}
  .circle-container {
    width: 78px;
    height: 78px;
    left: 80px;
    top: 90px;
    position: absolute;
}
.apply-leave-button {
    padding: 10px 20px;
    left: 198px;
    top: 35px;
    position: absolute;
    background-color: #FFA500;
    border: none;
    border-radius: 5px;
    color: #fff;
    font-size: 14px;
    font-weight: 500;
    font-family: 'Proxima Nova', sans-serif;
    cursor: pointer;
}
.legend {
    left: 25px;
    top: 315px;
    position: absolute;
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 15px;
    justify-content: center;
}
.all-card {
    width: 100%;
    /* padding: 54px; */
    margin: 0px;
}
.custom-request {
    width: 334px;
    padding: 15px;
    border-bottom: 1px solid #ddd;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.custom-container {
    width: 334px;
    height: 366px;
    background-color: #fff;
    border-radius: 15px;
    position: relative;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
}
.custom-title {
    color: #333;
    font-size: 10px;
    font-weight: 500;
    font-family: 'Proxima Nova', sans-serif;
}

  .search-boxs {
    width: 100%; /* Make the search box full-width in mobile view */
    max-width: 300px; /* Limit the maximum width */
  }
  .relative{
    display: none;
  }
  .logo {
    display: none;
}
.profile-detiles {
    width: 335px;
    float: right;
    margin: 20px;
    background-color: white;
    box-shadow: 0 8px 70px 0 #a9a9a9;
    border-radius: 10px;
    height: 366px;
    border: solid 1px #ffbb1e;
}
.top-content {
    background: antiquewhite;
    width: 333px;
    height: 155px;
    border-radius: 10px 10px 0px 0px;
}
.rounded-full {
    width: 56px;
    height: 56px;
    border-radius: 50%;
}

.profile-cards {
  width: 334px;
    float: right;
    margin: 20px;
    background-color: white;
    box-shadow: 0 8px 70px 0 #a9a9a9;
    border-radius: 10px;
    height: 366px;
    padding: 0px;
}
}


</style>
