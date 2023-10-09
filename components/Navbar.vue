<!-- Please remove this file from your project -->
<template>
  <div>

  <div class="">
    <div class="navbar">
      <!-- Left Section -->
      <div class="left-section">
          <div class="logo"><img src="../static/image 8.png"/></div>

      </div>

      <!-- Right Section -->
      <div class="right-section">
        <div class="notification icon">

              <input type="text" class="search-boxs" placeholder="Search" >
          </div>
          <div class="notification icon"><img src="../static/Restart Circle.svg"/></div>
          <div class="notification icon"><img src="../static/Bell.svg"/></div>
          <div class="profile icon" ><img @click="toggleProfileCard"  class="rounded-image" src="../static/profile.png" alt="Placeholder Image"><img class="relative" src="../static/Alt Arrow Down.svg" alt="Placeholder Image"></div>

      </div>

  </div>

  <div class="navbars navbars-ds">
        <div class="navbar-content">
            <div class="dash-menu">
                <div class=""><img class="link-icon" src="../static/Widget 7.png"/></div>
                <div class="">Dashboard</div>
                <div class=""><img class="link-icon" src="../static/Alt Arrow Down.png"/></div>
            </div>
            <div class="dash-menu">
                <div class=""><img class="link-icon" src="../static/State=Bold, Property 2=Building, Infrastructure, Property 3=Property 38.png"/></div>
                <div class="">Company Setups</div>
                <div class=""><img class="link-icon" src="../static/Alt Arrow Down.png"/></div>
            </div>
            <div class="dash-menu">
                <div class=""><img class="link-icon" src="../static/Calendar Mark.png"/></div>
                <div class="">Leave Tracker</div>
                <div class=""><img class="link-icon" src="../static/Alt Arrow Down.png"/></div>
            </div>
            <div class="dash-menu">
                <div class=""><img class="link-icon" src="../static/Users Group Two Rounded.svg"/></div>
                <div class="">Team/Department Calendar</div>
                <div class=""><img class="link-icon" src="../static/Alt Arrow Down.png"/></div>
            </div>
            <div class="dash-menu">
                <div class=""><img class="link-icon" src="../static/Settings.png"/></div>
                <div class="">Global Settings</div>
                <div class=""><img class="link-icon" src="../static/Alt Arrow Down.png"/></div>
            </div>

        </div>

        <div class="right-section"><img class="link-icon" src="../static/Maximize Square Minimalistic.svg"/></div>
    </div>
    <!-- Add this meta tag to ensure proper scaling on mobile devices -->
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<div class="navbars" v-show="togglemenucard">
    <div class="navbar-content">
        <div class="dash-menu">
            <div class=""><img class="link-icon" src="../static/Widget 7.png"/></div>
            <div class="">Dashboard</div>
            <div class=""><img class="link-icon" src="../static/Alt Arrow Down.png"/></div>
        </div>
        <div class="dash-menu">
            <div class=""><img class="link-icon" src="../static/State=Bold, Property 2=Building, Infrastructure, Property 3=Property 38.png"/></div>
            <div class="">Company Setups</div>
            <div class=""><img class="link-icon" src="../static/Alt Arrow Down.png"/></div>
        </div>
        <div class="dash-menu">
            <div class=""><img class="link-icon" src="../static/Calendar Mark.png"/></div>
            <div class="">Leave Tracker</div>
            <div class=""><img class="link-icon" src="../static/Alt Arrow Down.png"/></div>
        </div>
        <div class="dash-menu">
            <div class=""><img class="link-icon" src="../static/Users Group Two Rounded.svg"/></div>
            <div class="">Team/Department Calendar</div>
            <div class=""><img class="link-icon" src="../static/Alt Arrow Down.png"/></div>
        </div>
        <div class="dash-menu">
            <div class=""><img class="link-icon" src="../static/Settings.png"/></div>
            <div class="">Global Settings</div>
            <div class=""><img class="link-icon" src="../static/Alt Arrow Down.png"/></div>
        </div>

    </div>

    <div class="right-section"><img class="link-icon" src="../static/Maximize Square Minimalistic.svg"/></div>
</div>

<!-- Change the text for the link -->
<a class="navbars-mobile" @click="togglemenucard"><img src="../static/line.png"/></a>

  </div>
  <div class="profile-detiles" v-show="showProfileCard">
            <div class="top-content">
              <a><img @click="closeProfileCard"  class="link-icon" src="../static/close.png"/></a>
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
</div>
</template>

<script>

export default {
  name: 'NuxtNavbar',
  data() {
    return {
      showProfileCard: false,
    };
  },
  methods: {
  toggleProfileCard() {
    this.showProfileCard = !this.showProfileCard;
  },
  closeProfileCard() {
    this.showProfileCard = false; // Set showProfileCard to false to hide the card
  },
  // other methods...
},
};


</script>
<style>
/* styles.css */
.dash-menu{
    display: flex;
    margin-top: 5px;
    align-items: center;
}
/* styles.css */

/* Add a default bottom border line to .dash-menu */
.dash-menu {
    display: flex;
    margin-top: 5px;
    align-items: center;
    border-bottom: 3px solid transparent; /* Transparent border by default */
    transition: border-color 0.3s ease; /* Add a smooth transition effect */
}

/* Change the bottom border color on hover */
.dash-menu:hover {
    border-color: rgb(217,81,41);
    color: rgb(217,81,41); /* Change the border color on hover to your desired color (e.g., orange) */
}

/* Change the bottom border color when active (optional) */
.dash-menu:active {
    border-color: rgb(217,81,41);
    color: rgb(217,81,41); /* Change the border color when the menu item is active (e.g., when clicked) */
}


.dtl-info {
    width: 233px;
    height: 157px;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
    gap: 5px;
    display: inline-flex;
    padding: 20px;
}

.card-section {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
    gap: 2.5px;
}

.card-label {
    opacity: 0.60;
    color: #333; /* You can set your desired text color here */
    font-size: 13px;
    font-weight: medium;
    font-family: 'Proxima Nova', sans-serif;
}

.card-value {
    color: #333; /* You can set your desired text color here */
    font-size: 16px; /* You can adjust the font size as needed */
    font-weight: normal;
    font-family: 'Proxima Nova', sans-serif;
}

body{
  font-family: inherit;
}
.dtl-contant{
  padding: 10px;

}
.dtl-img{
  padding: 10px;
}
.link-icon{
  float: right;
    padding: 10px;
}
.profile-dtl{
  display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    padding: 17px;
  }
.rounded-full {
    width: 115px;
    height: 115px;
    border-radius: 50%; /* This makes the image rounded */
}

.top-content{
  background: antiquewhite;
    width: 445.5px;
    height: 155px;
    border-radius: 10px 10px 0px 0px;
}
/* Style for the profile card */
.profile-card {
  background-color: white;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

/* Show the profile card when v-show is true */
.profile-card[style*="display: block"] {
  display: block;
}
.profile-detiles {
  width: 447px;
    float: right;
    margin: 20px;
    background-color: white;
    box-shadow: 0 8px 70px 0 #a9a9a9;
    border-radius: 10px;
    height: 366px;
    border: solid 1px #ffbb1e;
}

.rounded-image {
    width: 50px;
    height: 50px;
    border-radius: 50%;
}

.search-boxs {
    background-image: url('../static/Magnifer.png');
    background-size: 20px;
    background-repeat: no-repeat;
    background-position: 309px center;
    padding-left: 40px;
    height: 40px;
    border: 1px solid #ccc;
    border-radius: 5px;
    width: 350px;
        }

.navbar {
    display: flex;
    justify-content: space-between;
    background-color: rgb(255, 255, 255) !important;
    padding: 10px;
    color: #ffffff;
    box-shadow: 0 8px 70px 0 #ededed;
}
/* styles.css */

.navbars {
  width: 100%;
    height: 50px;
    padding-left: 30px;
    background-color: #F7F7F7;
    box-shadow: inset 0px 0px 10px rgba(0, 0, 0, 0.2);
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 428px;
    display: inline-flex;
}

.navbar-content {
    display: flex;
    align-self: stretch;
    justify-content: center;
    align-items: center;
    display: inline-flex;
}

.nav-item {
    width: 149px;
    padding: 2.5px;
    border-bottom: 2px solid #FFA500; /* Replace with your desired border color */
    display: flex;
    justify-content: flex-start;
    align-items: center;
    gap: 2.5px;
}

.nav-icon {
    width: 5px;
    height: 5px;
    border-radius: 5px;
    /* Add your desired icon styles here */
}

.nav-text {
    color: #333; /* Replace with your desired text color */
    font-size: 13px;
    font-weight: medium;
    font-family: 'Proxima Nova', sans-serif;
}

/* Style for the last icon */
.nav-icon:last-child {
    width: 6px;
    height: 6px;
    border-radius: 5px;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
    flex: 1; /* To fill the remaining space */
}


/* Style for the left and right sections of the navbar */
.left-section {
  display: flex;
  align-items: center;
}

.right-section {
  display: flex;
  align-items: center;
}

/* Style for the logo */
.logo {
  margin-right: 20px;
}

/* Style for the search box */
.search-boxs {
  margin-right: 0px !important;
}

/* Style for the notification and profile icons */
.icon {
  margin-left: 20px;
}
@media screen and (max-width: 768px) {
  /* Mobile-specific styles here */
  .navbar {
    flex-direction: column; /* Stack elements vertically for mobile */
    align-items: center; /* Center items vertically in mobile view */
    padding: 20px; /* Increase padding for mobile spacing */
  }

  .left-section {
    margin-bottom: 10px; /* Add some spacing between sections in mobile view */
  }

  .right-section {
    margin-top: 10px; /* Add spacing above the right section in mobile view */
  }

  .logo {
    margin-right: 0; /* Remove margin for the logo in mobile view */
  }

  .icon {
    margin: 5px; /* Add spacing between icons in mobile view */
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
.navbars-mobile {
        display: flex;
        float: right;
    margin: 20px;
    }
    .navbars-ds {
        display: none;
    }

}
    @media (min-width: 768px) {
    .navbars-mobile {
        display: none;
    }
}


</style>
