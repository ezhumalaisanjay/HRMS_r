<!-- Please remove this file from your project -->
<template>

    <div class="">
      <div class="navbar">
        <!-- Left Section -->
        <div class="left-section">
            <div class="logo">Logo</div>
            <div class="search-box">
                <input type="text" placeholder="Search">
            </div>
        </div>

        <!-- Right Section -->
        <div class="right-section">
            <button class="add-button">Add</button>
            <div class="notification icon">Notification</div>
            <div class="profile icon">Profile</div>
        </div>
    </div>
    </div>
</template>

<script>
export default {
  name: 'NuxtTutorial'
}
</script>
<style>
/* Style for the navigation bar */
.navbar {
    display: flex;
    justify-content: space-between;
    background-color: #333;
    padding: 10px;
    color: white;
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
.search-box {
    margin-right: 20px;
}

/* Style for the notification and profile icons */
.icon {
    margin-left: 20px;
}
</style>
