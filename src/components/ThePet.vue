<template>
    <div class="pet">      
        <!-- <audio autoplay>
            <source src="../../public/demo.mp3" type="audio/mpeg"/>
        </audio>
        <button onclick="play()">播放题目</button>
        <audio controls class="audio-player"></audio>
        <button class="record-btn">开始回答</button>
        <a id="download" download="录音.ogg"></a>        -->
        <div class="lion">
            <embed src="../assets/学生狮子.svg" type="image/svg+xml"/>
        </div>
        <div class="blackboard">
            <div class="problem">
                {{question}}
            </div>
        </div>
    </div>
</template>

<script>
    export default {
		name:'UserInfo',
		data(){
			return {
				question:"82+49"
			}
		},
        methods:{
			// play(){
            //     var audioDom = document.querySelector("audio");
            //     audioDom.play();//播放音频
            // }
		},
	}
    // var audioDom = document.querySelector("audio");
    // function play(){
    //     audioDom.play();//播放音频
    // }  
    // //实现录音功能
    // const recordBtn=document.querySelector(".record-btn")
    // const player=document.querySelector(".audio-player")
    // const download=document.querySelector("#download")
    // if(navigator.mediaDevices.getUserMedia){
    //     let chunks = []
    //     const constraints={audio:true}
    //     navigator.mediaDevices.getUserMedia(constraints).then(
    //         stream =>{
    //             const mediaRecorder=new MediaRecorder(stream)
    //             recordBtn.onclick=()=>{
    //                 if(mediaRecorder.state=="recording"){
    //                     mediaRecorder.stop()
    //                     recordBtn.textContent="录音结束"
    //                 }else{
    //                     mediaRecorder.start()
    //                     recordBtn.textContent="录音中..."
    //                 }
    //             }
    //             mediaRecorder.ondataavailable=e=>{
    //                 chunks.push(e.data)
    //             }
    //             mediaRecorder.onstop=e=>{
    //                 const blob = new Blob(chunks,{type:"audio/ogg;codecs=opus"})
    //                 chunks=[]
    //                 const audioURL = window.URL.createObjectURL(blob)
    //                 player.src = audioURL
    //                 download.innerHTML="下载"
    //                 download.href=audioURL
    //             }
    //         },
    //         ()=>{
    //             console.error("授权失败！")
    //         }
    //     );
    // }else{
    //     console.error("浏览器不支持getUserMedia");
    // }
</script>

<style>
    .pet{
    width: 95vw;
    height: 53vh;
    }
    .lion{
        float: left;
        width: 40vw;
    }
    .lion embed{
        margin-top: 0vw;
        margin-left: 13vw;
        height: 50vh;
    }
    .blackboard{
        float: left;
        margin-left: -2vw;
        margin-top: 3vh;
        width: 44vw;
        height: 42.2vh;
        background-image: url("../assets/黑板.svg");
    }
    .blackboard .problem{
        margin-left: 9vw;
        margin-top: 12vh;
        font-size: 11vh;
        color: cornsilk;
    }
</style>