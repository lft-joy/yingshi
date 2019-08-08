<template>
    <footer id="footer">
        <ul>
            <router-link tag="li" to="/movie">
                <img src="@/assets/movie.png" alt="">
                <p>电影</p>
            </router-link>
            <router-link tag="li" to="/cinema">
                <img src="@/assets/CityHall.png"/>
                <p>影院</p>
            </router-link>
            <router-link tag="li" to="/mine">
                <img src="@/assets/personal.png" alt>
                <p>我的</p>
            </router-link>
        </ul>
    </footer>
</template>

<script>
    export default {}
</script>

<style lang="scss" scoped>
    #footer {
        width: 100%;
        height: 50px;
        background: white;
        border-top: 2px #ebe8e3 solid;
        position: fixed;
        left: 0;
        bottom: 0;
    }

    #footer ul {
        display: flex;
        text-align: center;
        height: 50px;
        align-items: center;
    }

    #footer ul li {
        flex: 1;
        height: 40px;
    }

    #footer ul li.active {
        color: #f03d37;
    }

    #footer ul li.router-link-active {
        color: #f03d37;
    }

    #footer ul i {
        font-size: 20px;
    }

    #footer ul p {
        font-size: 12px;
        line-height: 18px;
    }


  ul {
    width: 100%;
  }
  ul li {
    float: left;
    width: 33.3333%;
    height: 60px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
    ul li img {
        display: block;
        width: 18px;
        height: 18px;

    }

    ul li p {
        margin-top: 10px;
        font-size: 14px;
    }

    .router-link-active {
        color: red;
    }
</style>
