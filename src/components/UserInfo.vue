<template>
    <div class="info">
        <div class="title">
            <div class="head">
                <img src="../assets/cleverik.jpg" alt="ik">
            </div>
            <div class="level">
                {{LV}}
            </div>
        </div>
        <div class="name">
            <div class="username">{{name}}</div>
            <div class="exp">{{EXP}}</div>
        </div>
    </div>
</template>

<script>
    export default {
		name:'UserInfo',
		data(){
			return {
				LV:"Lv.100",
                name:'聪明的ik',
                EXP:"EXP:😎😎😎😎😎"
			}
		}
	}
</script>

<style>
    .info{
    margin-left: 1vw;
    margin-top: 2vh;
    height: 20vh;
    }
    .title{
        float: left;
        width: 15vh;
    }
    .head{
        height: 15vh;
        width: 15vh;
    }
    .head img{
        height: 15vh;
        border-radius: 50%;
    }
    .level{
        text-align: center;
        font-weight: 900;
        font-size: 3vh;
        line-height: 5vh;
    }
    .name{
        float:left;
        font-size: 2.5vh;
        font-family: 黑体;
        font-weight: 900;
        margin-top: 3vh;
        margin-left: 1.5vw;
    }
    .exp{
        margin-top: 2vh;
    }
</style>