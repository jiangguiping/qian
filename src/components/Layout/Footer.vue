<template>
    <footer class="footer has-text-grey-light has-background-grey-darker">
        <div class="container">
            <div>
                <span>更快 更高 更强</span>
                <span style="float:right">
                    <router-link :to="{path:'/admin/login'}">
                       管理员登录
                    </router-link>|
                    <a href="">百度</a>|
                    <a href="">blibli</a>
                </span>
            </div>
            <div>
                <span>{{title}}SUTURE MONSTER ALL</span>
                <div style="float: right">
                    <template>
                        <b-taglist attached>
                            <b-tag type="is-dark" size="is-normal">design</b-tag>
                            <b-tag type="is-info" size="is-normal">{{author}}</b-tag>
                        </b-taglist>
                    </template>
                </div>
            </div>
        </div>
        <back-top></back-top>
    </footer>
</template>

<script>
import BackTop from "@/components/Backtop/BackTop";
export default {
    name: 'Footer',
    data() {
        return {
            title: "© " + new Date().getFullYear() + ' 阿猫',
            author:'阿猫'
        };
    },
    components: {
        BackTop
    },
  
};
</script>

<style  scoped>
footer {
  margin-top: 120px;
  height: 150px;
}
footer a{
  color: #bfbfbf;
}

</style>