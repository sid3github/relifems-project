<template>
    <div class="dashboard-section">
        <div class="dashboard-section-one">
            <h5>Your Earning</h5>
            <div class="sub-one">
                <div class="dashboard-section-one-img">
                    <img src="../assets/circle-chart.svg" alt="pie-chart" />
                </div>
                <div class="dashboard-section-one-text">
                    <h1><sup>$</sup> 98.00</h1>
                    <p>
                        <span><i class="fas fa-minus diff-color"></i></span>
                        Graphics
                    </p>
                    <p>
                        <span><i class="fas fa-minus"></i></span> Interfaces
                    </p>
                </div>
                <div class="dashboard-section-one-diagram">
                    <img src="../assets/small-graph.svg" alt="small-graph" />
                </div>
            </div>
        </div>
        <div class="dashboard-section-two">
            <div class="sub-two">
                <div class="best-month-box">
                    <h5>Your Best Month</h5>
                    <div class="best-month">
                        <div class="best-month-img">
                            <i class="far fa-sun"></i>
                        </div>
                        <div class="best-month-text">
                            <h4>$24.89</h4>
                            <span>February</span>
                        </div>
                        <div class="best-month-button">
                            <i class="fas fa-ellipsis-v"></i>
                        </div>
                    </div>
                </div>
                <div class="best-tool-box">
                    <h5>Your Best Tool</h5>
                    <div class="best-tool">
                        <div class="best-tool-img">
                            <i class="fas fa-drafting-compass"></i>
                        </div>
                        <div class="best-tool-text">
                            <h4>$129.00</h4>
                            <span>Sketch App</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="dashboard-section-three">
            <h5>Your Top Item</h5>
            <div class="sub-three">
                <div class="sub-three-title">
                    <div class="sub-three-product">Product</div>
                    <div class="sub-three-earning">Earning</div>
                </div>
                <div class="sub-three-item">
                    <div class="item-img">
                        <!-- <img src="../assets/product.svg" alt="product" /> -->
                        <i class="fab fa-product-hunt"></i>
                    </div>
                    <div class="item-text">
                        <h4>Thefox 6 Template</h4>
                        <span>Sketch App</span>
                    </div>
                    <div class="item-price">
                        <span>$17.58</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "DashboardSection",
};
</script>

<style>
.dashboard-section {
    display: grid;
    grid-template-rows: 40% 20% 40%;
    grid-gap: 1rem;
}

.dashboard-section-one h5,
.dashboard-section-two h5,
.dashboard-section-three h5 {
    margin: 14px auto;
    color: grey;
    font-weight: 200;
}

.sub-one {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #fff;
    height: 150px;
    border-radius: 14px;
}

.dashboard-section-one-img img {
    max-width: 150px;
    margin: 15px 30px;
}

.dashboard-section-one-text h1 {
    font-size: 40px;
    font-weight: 300;
}

.dashboard-section-one-text p {
    font-size: 12px;
    margin: 10px auto;
}

.dashboard-section-one-text p span {
    margin-right: 10px;
}

.diff-color {
    color: rgb(236 187 198) !important;
}

.dashboard-section-one-diagram img {
    max-width: 75px;
    border: 1px solid white;
    background: #5a5aa5;
    border-radius: 14px;
    margin: 6px 4px 0px 4px;
    padding: 40px 2px;
}

sup {
    font-size: 24px;
}

.sub-two {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 2rem;
}

.best-month {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: #fff;
    height: 100px;
    border-radius: 14px;
    box-shadow: 0px 34px 34px #c1c1c1;
}

.best-month-img {
    padding: 6% 8%;
    border: 1px solid;
    border-radius: 100%;
    margin: 10px;
    background: #f6edbe;
}

.best-month-text {
    margin-right: 2rem;
}

.best-month-text span {
    font-size: 12px;
    color: grey;
}

.best-month-button {
    display: flex;
    align-items: center;
    padding: 16px;
    background: #f9f9fe;
    height: 90px;
    margin: 6px;
    border-radius: 13px;
}

.best-tool {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: #464678;
    height: 100px;
    border-radius: 14px;
}

.best-tool-img {
    border-radius: 100%;
    padding: 6% 8%;
    background: #6464ac;
    margin: 10px;
}

.best-tool-text {
    margin-right: 6rem;
}

.best-tool-text h4 {
    color: #fff;
    font-weight: 200;
    font-size: 14px;
}

.best-tool-text span {
    font-size: 10px;
    color: grey;
}

.dashboard-section-three {
    position: relative;
    top: 3rem;
    overflow: hidden;
    height: 68%;
}

.sub-three {
    background: #fff;
    height: 150px;
    border-radius: 14px;
    padding: 8px;
}

.sub-three-title {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-radius: 10px;
    padding: 10px;
    background: #f4f4fc;
    font-size: 12px;
    color: grey;
}

.sub-three-product {
    margin-left: 2rem;
}
.sub-three-earning {
    margin-right: 4rem;
}

.sub-three-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.sub-three-item .item-img {
    padding: 2% 3%;
    border: 1px solid;
    border-radius: 100%;
    margin: 10px;
    margin-left: 2rem;
    background: #d8ecff;
}
/* .sub-three-item .item-img i {
    max-width: 5px;
    height: 5px;
} */

.item-text {
    margin-right: 8rem;
    font-size: 12px;
}

.item-price {
    margin-bottom: 1.5rem;
    margin-right: 5rem;
    font-size: 14px;
    font-weight: 600;
}
</style>