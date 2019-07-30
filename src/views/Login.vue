<template>
    <div class="Login">
        <div class="form">
            <h3>Login Form</h3>
            <div>
                <i class="el-icon-user-solid"></i>
                <el-input
                        placeholder="请输入用户名"
                        v-model="userName">
                </el-input>
            </div>
            <div>
                <i class="el-icon-lock"></i>
                <el-input
                        placeholder="请输入密码"
                        v-model="password"
                        show-password>
                </el-input>
                <i class="el-icon-view" :class="el-icon-c-scale-to-origina"></i>
            </div>

            <el-button type="primary">Login</el-button>
        </div>
    </div>
</template>
<script>
    export default {
        data(){
            return{
                userName:'',
                password:''
            }
        }
    }
</script>
<style>
    .Login{
        display: flex;
        justify-content: center;
        width:100%;
        height:100%;
        background:#283443;
        color:#fff;
    }
    .form{
        width:520px;
        max-width: 100%;
        padding:160px 35px 0;
    }
    .form h3{
        font-size: 26px;
        color:#eee;
        margin:0 auto 40px auto;
    }
    .Login .el-input{

    }
    .Login .el-input__inner{
        border:1px solid rgba(255,255,255,0.1);
        background:rgba(0,0,0,0.1);
        border-radius: 5px;
        line-height: 47px;
        height:47px;
        color:#fff;
        margin-bottom: 22px;
    }
    .Login .el-button{
        width:100%;
    }
</style>
