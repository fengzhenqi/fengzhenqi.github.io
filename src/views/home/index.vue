<template>
  <div class="home">
        <div class="nav-list">
            <h1>冯小草个人网站</h1>
            <ul>
                <li v-for="item in list" @click="goRouter(item.path)">{{item.name}}</li>
            </ul>
        </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            list: [
                {name: '常用网站', path: '/net'},
                {name: '博文', path: '/net'},
                {name: '其他', path: '/net'},
            ]
        }
    },
    methods: {
        goRouter(val) {
            console.log(val);
            this.$router.push({path: val});
        }
    },
}
</script>

<style lang="less" scoped>
.home {
    width: 100%;
    height: 100%;
    background: rgba(100, 121, 235, .7);
    position: relative;

    .nav-list {
        box-sizing: border-box;
        padding: 10px 24px;
        width: 30%;
        min-width: 300px;
        border: 1px solid #eee;
        border-radius: 5px;
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);
        background: rgba(0, 0, 0, .4);
        color: #fff;

        h1 {
            text-align: center;
            height: 40px;
            line-height: 40px;
            border-bottom: 1px solid #eee;
            margin-bottom: 5px;
        }

        ul {
            width: 100%;
            height: 100%;

            li {
                width: 100%;
                height: 40px;
                line-height: 40px;
                border-radius: 5px;
                cursor: pointer;
                &:hover {
                    background: #fff;
                    color: #42b983;
                }
            }

        }

        
    }
}
</style>