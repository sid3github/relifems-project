<template>
    <div class="outer-container">
        <div class="main-box">
            <div class="main-grid">
                <div class="sidebar-layout">
                    <div class="sidenav">
                        <div class="sidenav-title">
                            <h3>Interface</h3>
                            <i class="fas fa-grip-horizontal"></i>
                        </div>
                        <div class="nav-links">
                            <ul>
                                <li>
                                    <i class="fas fa-th-large"></i>
                                    <p>Dashboard</p>
                                </li>
                                <li>
                                    <i class="fas fa-address-card"></i>
                                    <p>Profile</p>
                                </li>
                                <li>
                                    <i class="fas fa-tools"></i>
                                    <p>Setting</p>
                                </li>
                                <li>
                                    <i class="fas fa-cloud-upload-alt"></i>
                                    <p>Cloud</p>
                                </li>
                                <li>
                                    <i class="fas fa-comment-alt"></i>
                                    <p>Message</p>
                                </li>
                            </ul>
                        </div>
                        <div class="new-item-box">
                            <div class="item-box">
                                <i class="fas fa-plus"></i>
                                <p>New Item</p>
                            </div>
                            <div class="item-box-content">
                                <p>Click '+' to create your new items</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="content-layout">
                    <SearchSection />
                    <div class="content-grid-section">
                        <BannerSection />
                        <DashboardSection />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import BannerSection from "./components/BannerSection.vue";
import DashboardSection from "./components/DashboardSection.vue";
import SearchSection from "./components/SearchSection.vue";

export default {
    name: "App",
    components: {
        BannerSection,
        DashboardSection,
        SearchSection,
    },
};
</script>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Poppins", sans-serif;
}

body {
    background: rgb(247 221 227);
}

.outer-container {
    margin: 3rem;
}

.main-box {
    background: #fff;
    border-radius: 14px;
}

.main-grid {
    display: grid;
    grid-template-columns: 15% auto;
}

.fa-grip-horizontal {
    border-radius: 50%;
    background: #ebebf8;
    padding: 6px;
    font-size: 18px;
}

.sidenav-title {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    font-size: 14px;
    margin: 20px 20px 40px 20px;
}

.nav-links {
    width: 125px;
    margin: 0 auto;
}

.nav-links ul li {
    display: flex;
    align-items: center;
    list-style: none;
    margin: 8px auto;
    cursor: pointer;
    padding: 12px 6px;
}

.nav-links ul li:hover {
    background: rgb(247 221 227);
    border-radius: 14px;
}

.nav-links li p {
    margin-left: 24px;
    color: grey;
    font-size: 12px;
}

.nav-links li p:hover {
    color: #000;
    font-weight: bold;
}

.fas {
    color: #8787fd;
}

.new-item-box {
    background: #f9f9fe;
    padding: 15px 20px;
    border-radius: 14px;
    margin: 40px 8px 8px 8px;
}

.item-box {
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    list-style: none;
    margin: 8px auto;
    padding: 12px 6px;
    color: #000;
    font-size: 12px;
    font-weight: bold;
    background: rgb(234 235 255);
    border-radius: 14px;
    width: 125px;
}

.item-box-content {
    margin: 20px auto;
    width: 125px;
}

.item-box-content p {
    font-size: 10px;
    text-align: center;
    color: grey;
}

.content-layout {
    margin: 8px;
    border-radius: 12px;
    background: #f4f4fc;
}

.content-grid-section {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 3rem;
    margin: 5px 20px;
}

@media screen and (max-width: 998px) {
    .outer-container {
        margin: unset;
    }

    .main-grid {
        display: block;
        grid-template-columns: unset;
    }

    /* .sidebar-layout {
        display: none;
    } */

    .content-layout {
        margin: unset;
    }

    .search-section {
        max-width: unset;
        margin-left: unset;
        margin-right: unset;
    }

    .menu {
        display: unset;
    }

    .searchTerm {
        width: unset;
    }

    .notify {
        margin-left: unset;
    }

    .profile-img {
        margin-left: unset;
    }

    .content-grid-section {
        display: unset;
        grid-template-columns: unset;
        grid-gap: unset;
        text-align: center;
    }

    .banner-btns {
        justify-content: center;
    }

    .banner-content-img {
        margin-left: unset;
    }

    .banner-content-btn button {
        width: 150px;
    }

    .dashboard-section {
        display: unset;
    }

    .dashboard-section-one {
        margin-top: 5rem;
    }

    .sub-one {
        margin: 20px;
    }

    .dashboard-section-one-img img {
        margin: unset;
    }

    .dashboard-section-one-text h1 {
        font-size: unset;
    }

    .sub-two {
        display: unset;
        grid-template-rows: unset;
        grid-gap: unset;
    }

    .best-month-box,
    .best-tool-box {
        margin: 20px;
    }

    .dashboard-section-three {
        top: 50%;
        overflow: unset;
        height: fit-content;
    }

    .sub-three {
        padding: 4px;
    }
}
</style>
