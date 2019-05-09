<template>
  <section class="container">
    <div>
      <a-form>
        <a-form-item
          label="综合信息查询"
          :label-col="{ span: 6 }"
          :wrapper-col="{ span: 12 }"
        >
          <a-input-search enter-button style="width:250px" @search="onSearch" />
        </a-form-item>
      </a-form>
    </div>
    <div style="margin-left: 15px">
      <div
        :style="{
          color: 'rgb(28, 97, 162)',
          paddingBottom: '10px'
        }"
      >
        <span
          :style="{
            float: 'left',
            fontSize: '18px'
          }"
          >招标公告(851)
        </span>
        <a :style="{ float: 'right', marginRight: '10px' }">更多</a>
      </div>
      <a-divider />
      <a-list item-layout="horizontal" :split="false">
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-05-08</span>
          <a-list-item-meta description="050801招投标">
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-05-06</span>
          <a-list-item-meta description="0506招投标">
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-05-05</span>
          <a-list-item-meta description="0505招投标">
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-04-24</span>
          <a-list-item-meta description="042401招投标">
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-04-18</span>
          <a-list-item-meta description="0418招投标">
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-04-08</span>
          <a-list-item-meta description="040801招投标">
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-03-08</span>
          <a-list-item-meta description="030801招投标">
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-03-28</span>
          <a-list-item-meta description="032801招投标">
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
      </a-list>
    </div>
    <div :style="{ marginTop: '20px', marginLeft: '15px' }">
      <div
        :style="{
          color: 'rgb(28, 97, 162)',
          paddingBottom: '10px'
        }"
      >
        <span
          :style="{
            float: 'left',
            fontSize: '18px'
          }"
          >询价公告(238)
        </span>
        <a :style="{ float: 'right', marginRight: '10px' }">更多</a>
      </div>
      <a-divider />
      <a-list item-layout="horizontal" :split="false">
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-04-24</span>
          <a-list-item-meta description="张家港油漆询价询比价公告">
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-04-24</span>
          <a-list-item-meta description="张家港公司空压机配件采购询比价公告">
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-04-28</span>
          <a-list-item-meta description="张家港公司制氮机组配件采购询比价公告">
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-05-08</span>
          <a-list-item-meta description="久泰内蒙古公司五金杂品采购询比价公告">
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-05-08</span>
          <a-list-item-meta
            description="工程部高强螺栓（请购单1463）询比价公告"
          >
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-05-08</span>
          <a-list-item-meta
            description="内蒙古公司药剂类（5月三氯化铁）询比价公告"
          >
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
        <a-list-item>
          <span slot="actions" style="margin-right:20px">2019-05-08</span>
          <a-list-item-meta
            description="内蒙古公司阀门类（气动钨钢旋转阀）询比价公告"
          >
            <a-avatar
              slot="avatar"
              :style="{
                marginTop: '-5px',
                marginRight: '-15px',
                background: '#fff',
                color: 'lightgray'
              }"
            >
              <a-icon type="caret-right" theme="filled" />
            </a-avatar>
          </a-list-item-meta>
        </a-list-item>
      </a-list>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    onSearch() {}
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  /* min-height: 100vh; */
  /* display: flex; */
  justify-content: center;
  /* align-items: center; */
  /* text-align: center; */
  background: #fff;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
