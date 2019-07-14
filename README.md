# demo
vue demo
---
- **vue-cli3构建项目**      `vue create xxx`
    - **添加vue-router**    `vue add router`
    - **添加vuex**          `vue add vuex`
    - **添加element**       `vue add element`
    - **添加less**          `npm/cnpm install less less-loader --save`
    - **引入全局less变量**  `vue add style-resources-loader`
        - vue.config.js中设置
        ``` 
        const path = require('path')
        module.exports = {
            pluginOptions: {
                'style-resources-loader': {
                    preProcessor: 'less',
                    patterns: [
                        path.resolve(__dirname, './src/assets/public.less') // 引号内为公共less文件引入地址
                    ]
                }
            }
        }
        ``` 


