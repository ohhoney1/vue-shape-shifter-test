<template>
    <div id='ywy' class='wrap'>
        <canvas class="canvas"></canvas>
    </div>
</template>

<script>
    import ss from './shape-shifter.js'

    export default{
        name: 'shape-shifter',
        props: {
            content: {
                type: String,
                default: 'hello world'
            },
            width: {
                type: Number,
                default: 1000
            },
            height: {
                type: Number,
                default: 600
            }
        },
        data(){
            return{

            }
        },
        mounted() {
            ss(this.content, this.width, this.height);
        }
    }
</script>

<style>
    #ywy {
        width: 100%;
        height: 100%;
        position: absolute;
        text-align: center;
        line-height: 100%;
    }
    .wrap {
        background-color: #69b4ca;
        /*background: -webkit-linear-gradient(top, rgb(203, 235, 219) 0%, rgb(55, 148, 192) 120%);
        background: -moz-linear-gradient(top, rgb(203, 235, 219) 0%, rgb(55, 148, 192) 120%);
        background: -o-linear-gradient(top, rgb(203, 235, 219) 0%, rgb(55, 148, 192) 120%);
        background: -ms-linear-gradient(top, rgb(203, 235, 219) 0%, rgb(55, 148, 192) 120%);
        background: linear-gradient(top, rgb(203, 235, 219) 0%, rgb(55, 148, 192) 120%);*/
    }
</style>
