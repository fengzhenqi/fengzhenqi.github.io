<template>
  <div class="net">
    <div class="net-content">
      <h2>开发</h2>
      <ul>
        <li v-for="(item, index) in list" :key="index" @click="open(item.url)">{{item.name}}</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      list: [
        {
          name: 'VUE文档',
          url: 'https://vuejs.bootcss.com/api/'
        },
        {
          name: 'webpack',
          url: 'https://www.webpackjs.com/configuration/'
        },
        {
          name: 'element-ui',
          url: 'https://element.eleme.cn/#/zh-CN/component/installation'
        },
        {
          name: 'vue-cli',
          url: 'https://cli.vuejs.org/zh/guide/cli-service.html'
        },
        {
          name: 'momentjs时间处理',
          url: 'http://momentjs.cn/'
        },
        {
          name: 'Threejs中文网',
          url: 'http://www.webgl3d.cn/'
        },
        {
          name: 'deck.gl',
          url: 'https://github.com/visgl/deck.gl/blob/master/docs/README.md'
        },
        {
          name: '百度地图SDK',
          url: 'http://lbsyun.baidu.com/index.php?title=webapi'
        },
        {
          name: 'unapp官网',
          url: 'https://uniapp.dcloud.io/'
        },
        {
          name: 'flv.js视频流',
          url: 'https://github.com/Bilibili/flv.js'
        },
        {
          name: 'hls.js视频流',
          url: 'https://github.com/video-dev/hls.js/blob/master/docs/API.md'
        },
        {
          name: 'video标签',
          url: 'https://www.runoob.com/tags/tag-video.html'
        },
        {
          name: 'pug模板语言',
          url: 'https://www.pugjs.cn/api/getting-started.html'
        },
        {
          name: 'npm官网',
          url: 'https://www.npmjs.cn/cli/run-script/'
        },
        {
          name: 'ImageOptim图片压缩工具',
          url: 'https://imageoptim.com/howto.html'
        },
        {
          name: 'Linux命令',
          url: 'https://www.runoob.com/linux/linux-command-manual.html'
        },
        {
          name: '百度Composer仓库',
          url: 'http://composer.baidu.com/'
        },
        {
          name: 'ps软件',
          url: 'https://www.didixk.com/15912.html'
        },
        {
          name: '墨刀',
          url: 'https://modao.cc/downloads'
        },
        {
          name: 'mockjs',
          url: 'http://mockjs.com/'
        },
        {
          name: '图片文字提取',
          url: 'http://ocrmaker.com/'
        },
        {
          name: 'echarts图标',
          url: 'https://echarts.apache.org/zh/index.html'
        },
        {
          name: 'echarts图标',
          url: 'https://echarts.apache.org/zh/index.html'
        },
        {
          name: 'mongoosejs',
          url: 'http://www.mongoosejs.net/docs/guide.html'
        },
        {
          name: 'mongoosejs',
          url: 'http://www.mongoosejs.net/docs/guide.html'
        },
        {
          name: 'jquery',
          url: 'https://jquery.com/'
        },
        {
          name: 'express',
          url: 'https://www.expressjs.com.cn/starter/generator.html'
        },
        {
          name: 'nginx代理服务',
          url: 'https://www.nginx.cn/install'
        },
        
      ]
    }
  },
  methods: {
    open(url) {
      window.open(url);
    }
  }
}
</script>

<style lang="less" scoped>
.net {
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, .4);
  

  h2 {
    text-align: center;
    font-size: 28px;
    height: 40px;
    line-height: 40px;
  }

  .net-content {
    width: 80%;
    min-height: calc(100% - 40px);
    background: #fff;
    padding: 24px;
    box-sizing: border-box;
    border-radius: 20px 0px 20px 0px;
    position: absolute;
    left: 10%;
    top: 20px;
    overflow: hidden;
    
    ul {
      width: 100%;
      height: 100%;

      li {
        width: 50%;
        height: 40px;
        line-height: 40px;
        float: left;
        text-align: center;
        cursor: pointer;
        color: rgb(243, 128, 51);
        &:hover {
          color: #42b983;
        }
      }
    }
  }
}
</style>
