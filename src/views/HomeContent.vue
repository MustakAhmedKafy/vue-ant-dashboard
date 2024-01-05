<script setup>
import { ArrowUpOutlined } from '@ant-design/icons-vue'
</script>
<template>
  <a-row :gutter="16">
    <a-col :sm="6" :span="24">
      <a-card class="card" title="TOTAL TRAFFIC" :bordered="false">
        <template style="display: flex; justify-content: space-between">
          <p style="font-size: 18px; font-weight: bold">350,897</p>
          <p class="card-icon"><img src="/icons8-one-finger-skin-type-1-48.png" alt="" /></p>
        </template>
        <div>
          <span style="color: #2dce89; padding-right: 5px"><ArrowUpOutlined /> 3.48%</span>
          <span>Since last month</span>
        </div>
      </a-card>
    </a-col>
    <a-col :sm="6" :span="24">
      <a-card class="card" title="TOTAL TRAFFIC" :bordered="false">
        <template style="display: flex; justify-content: space-between">
          <p style="font-size: 18px; font-weight: bold">2,356</p>
          <p class="card-icon card-icon2">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="18"
              height="18"
              fill="currentColor"
              class="bi bi-pie-chart-fill"
              viewBox="0 0 16 16"
            >
              <path
                d="M15.985 8.5H8.207l-5.5 5.5a8 8 0 0 0 13.277-5.5zM2 13.292A8 8 0 0 1 7.5.015v7.778zM8.5.015V7.5h7.485A8 8 0 0 0 8.5.015"
              />
            </svg>
          </p>
        </template>
        <div>
          <span style="color: #2dce89; padding-right: 5px"><ArrowUpOutlined /> 12.18%</span>
          <span>Since last month</span>
        </div>
      </a-card>
    </a-col>
    <a-col :sm="6" :span="24">
      <a-card class="card" title="SALES" :bordered="false">
        <template style="display: flex; justify-content: space-between">
          <p style="font-size: 18px; font-weight: bold">924</p>
          <p class="card-icon card-icon3">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="18"
              height="18"
              fill="currentColor"
              class="bi bi-cash-coin"
              viewBox="0 0 16 16"
            >
              <path
                fill-rule="evenodd"
                d="M11 15a4 4 0 1 0 0-8 4 4 0 0 0 0 8m5-4a5 5 0 1 1-10 0 5 5 0 0 1 10 0"
              />
              <path
                d="M9.438 11.944c.047.596.518 1.06 1.363 1.116v.44h.375v-.443c.875-.061 1.386-.529 1.386-1.207 0-.618-.39-.936-1.09-1.1l-.296-.07v-1.2c.376.043.614.248.671.532h.658c-.047-.575-.54-1.024-1.329-1.073V8.5h-.375v.45c-.747.073-1.255.522-1.255 1.158 0 .562.378.92 1.007 1.066l.248.061v1.272c-.384-.058-.639-.27-.696-.563h-.668zm1.36-1.354c-.369-.085-.569-.26-.569-.522 0-.294.216-.514.572-.578v1.1zm.432.746c.449.104.655.272.655.569 0 .339-.257.571-.709.614v-1.195z"
              />
              <path
                d="M1 0a1 1 0 0 0-1 1v8a1 1 0 0 0 1 1h4.083q.088-.517.258-1H3a2 2 0 0 0-2-2V3a2 2 0 0 0 2-2h10a2 2 0 0 0 2 2v3.528c.38.34.717.728 1 1.154V1a1 1 0 0 0-1-1z"
              />
              <path d="M9.998 5.083 10 5a2 2 0 1 0-3.132 1.65 6 6 0 0 1 3.13-1.567" />
            </svg>
          </p>
        </template>
        <div>
          <span style="color: #e81616; padding-right: 5px"><ArrowUpOutlined /> 5.72%</span>
          <span>Since last month</span>
        </div>
      </a-card>
    </a-col>
    <a-col :sm="6" :span="24">
      <a-card class="card" title="PERFORMANCE" :bordered="false">
        <template style="display: flex; justify-content: space-between">
          <p style="font-size: 18px; font-weight: bold">54.8%</p>
          <p class="card-icon card-icon4">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="18"
              height="18"
              fill="currentColor"
              class="bi bi-bar-chart-fill"
              viewBox="0 0 16 16"
            >
              <path
                d="M1 11a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1v3a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1zm5-4a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1v7a1 1 0 0 1-1 1H7a1 1 0 0 1-1-1zm5-5a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1v12a1 1 0 0 1-1 1h-2a1 1 0 0 1-1-1z"
              />
            </svg>
          </p>
        </template>
        <div>
          <span style="color: #2dce89; padding-right: 5px"><ArrowUpOutlined /> 49,65%</span>
          <span>Since last month</span>
        </div>
      </a-card>
    </a-col>
  </a-row>
</template>

<style scoped>
.card-icon {
  background: linear-gradient(87deg, #f5365c, #f56036) !important;
  height: 45px;
  width: 45px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
}

.card-icon img {
  height: 25px;
  width: 25px;
}
.card-icon.card-icon2 {
  background: linear-gradient(87deg,#fb6340,#fbb140)!important;
  color: white;
}
.card-icon.card-icon3 {
  background: linear-gradient(87deg, #2dce89, #2dcecc) !important;
  color: white;
}
.card-icon.card-icon4 {
  background: linear-gradient(87deg, #11cdef, #1171ef) !important;
  color: white;
}

.card {
  width: 300px;
  height: 143px;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  /* background: linear-gradient(45deg, #4CAF50, #2196F3); */
  color: #000;
  /* display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center; */
  /* text-align: center; */
}

.card h2 {
  margin: 0;
}

.card p {
  margin: 10px 0 0;
}
</style>
