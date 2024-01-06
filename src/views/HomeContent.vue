<script setup>
import { ref } from "vue";
import { ArrowUpOutlined } from '@ant-design/icons-vue';

const cards = ref([
      {
        title: 'TOTAL TRAFFIC',
        class: 'card',
        value: '350,897',
        iconClass: 'card-icon card-icon1',
    icon:
     ` <svg
              fill="#ffffff"
              height="18px"
              width="18px"
              version="1.1"
              id="Layer_1"
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
              viewBox="0 0 512 512"
              xml:space="preserve"
            >
              <g>
                <g>
                  <path
                    d="M436.312,79.026c-5.531-7.376-15.996-8.872-23.373-3.339l-125.31,93.983l-57.553-28.777
			c-5.656-2.829-12.426-2.219-17.484,1.576L79.026,242.643c-7.376,5.533-8.872,15.998-3.339,23.374
			c3.28,4.374,8.293,6.679,13.37,6.679c3.485,0,7.001-1.089,10.004-3.34l125.31-93.983l57.553,28.777
			c5.655,2.828,12.425,2.218,17.484-1.576L432.973,102.4C440.349,96.867,441.845,86.402,436.312,79.026z"
                  />
                </g>
              </g>
              <g>
                <g>
                  <path
                    d="M456.348,0H55.652C24.966,0,0,24.966,0,55.652v400.696C0,487.034,24.966,512,55.652,512h400.696
			C487.034,512,512,487.034,512,456.348V55.652C512,24.966,487.034,0,456.348,0z M478.609,456.348
			c0,12.275-9.986,22.261-22.261,22.261h-16.696V189.217c0-9.22-7.475-16.696-16.696-16.696c-9.22,0-16.696,7.475-16.696,16.696
			v289.391H372.87V239.304c0-9.22-7.475-16.696-16.696-16.696c-9.22,0-16.696,7.475-16.696,16.696v239.304h-33.391V289.391
			c0-9.22-7.475-16.696-16.696-16.696s-16.696,7.475-16.696,16.696v189.217h-33.391v-222.61c0-9.22-7.475-16.696-16.696-16.696
			s-16.696,7.475-16.696,16.696v222.61h-33.391V306.087c0-9.22-7.475-16.696-16.696-16.696s-16.696,7.475-16.696,16.696v172.522
			h-33.391V356.174c0-9.22-7.475-16.696-16.696-16.696c-9.22,0-16.696,7.475-16.696,16.696v122.435H55.652
			c-12.275,0-22.261-9.986-22.261-22.261V55.652c0-12.275,9.986-22.261,22.261-22.261h400.696c12.275,0,22.261,9.986,22.261,22.261
			V456.348z"
                  />
                </g>
              </g>
            </svg>`,
        color: '#2dce89',
        percentage: '3.48%',
        since: 'Since last month',
      },
      {
        title: 'TOTAL TRAFFIC',
        class: 'card',
        value: '2,356',
        iconClass: 'card-icon card-icon2',
        icon: ` <svg
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
            </svg>`,
        color: '#2dce89',
        percentage: '12.18%',
        since: 'Since last month',
      },
      {
        title: 'SALES',
        class: 'card',
        value: '924',
        iconClass: 'card-icon card-icon3',
        icon:  `<svg
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
            </svg>`,
        color: '#e81616',
        percentage: '5.72%',
        since: 'Since last month',
      },
      {
        title: 'PERFORMANCE',
        class: 'card',
        value: '54.8%',
        iconClass: 'card-icon card-icon4',
        icon: ` <svg
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
            </svg>`,
        color: '#2dce89',
        percentage: '49.65%',
        since: 'Since last month',
      },
    ]);
</script>
<template>
  <!-- <a-row :gutter="16">
    <a-col :sm="6" :span="24">
      <a-card class="card" title="TOTAL TRAFFIC" :bordered="false">
        <template style="display: flex; justify-content: space-between">
          <p style="font-size: 18px; font-weight: bold">350,897</p>
          <p class="card-icon card-icon1">
            
          </p>
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
           
          </p>
        </template>
        <div>
          <span style="color: #2dce89; padding-right: 5px"><ArrowUpOutlined /> 49,65%</span>
          <span>Since last month</span>
        </div>
      </a-card>
    </a-col>
  </a-row> -->
  <a-row :gutter="16">
    <a-col v-for="(card, index) in cards" :key="index" :sm="6" :span="24">
      <a-card :class="card.class" :title="card.title" :bordered="false">
        <template style="display: flex; justify-content: space-between">
          <p style="font-size: 18px; font-weight: bold">{{ card.value }}</p>
          <p :class="card.iconClass">
            <span v-html="card.icon"></span>
          </p>
        </template>
        <div>
          <span :style="{ color: card.color, 'padding-right': '5px' }">
            <ArrowUpOutlined /> {{ card.percentage }}
          </span>
          <span>{{ card.since }}</span>
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
  color: white;
}
.card-icon.card-icon1 {
  background: linear-gradient(87deg, #f5365c, #f56036) !important;
}
.card-icon1 svg {
  color: #fff;
}
.card-icon.card-icon2 {
  background: linear-gradient(87deg, #fb6340, #fbb140) !important;
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
