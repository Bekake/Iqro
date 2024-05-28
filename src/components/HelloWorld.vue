<template>
<div class="mainconatiner">
  <div class="bars">
    <div class="logo">
      <svg width="22" height="16" viewBox="0 0 22 16" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path fill-rule="evenodd" clip-rule="evenodd" d="M-3.05176e-05 1.45455C-3.05176e-05 0.651222 0.651192 0 1.45451 0H9.45452C10.2578 0 10.9091 0.651222 10.9091 1.45455C10.9091 2.25787 10.2578 2.90909 9.45452 2.90909H1.45451C0.651192 2.90909 -3.05176e-05 2.25787 -3.05176e-05 1.45455Z" fill="#51459E"/>
        <path fill-rule="evenodd" clip-rule="evenodd" d="M-3.05176e-05 7.99999C-3.05176e-05 7.19666 0.651192 6.54544 1.45451 6.54544H19.6363C20.4397 6.54544 21.0909 7.19666 21.0909 7.99999C21.0909 8.80331 20.4397 9.45453 19.6363 9.45453H1.45451C0.651192 9.45453 -3.05176e-05 8.80331 -3.05176e-05 7.99999Z" fill="#51459E"/>
        <path fill-rule="evenodd" clip-rule="evenodd" d="M-3.05176e-05 14.5455C-3.05176e-05 13.7421 0.651192 13.0909 1.45451 13.0909H16.7272C17.5306 13.0909 18.1818 13.7421 18.1818 14.5455C18.1818 15.3488 17.5306 16 16.7272 16H1.45451C0.651192 16 -3.05176e-05 15.3488 -3.05176e-05 14.5455Z" fill="#51459E"/>
      </svg>
    </div>
    <div class="buttons">
      <div :class="['mybutton', {active: activeindex == 1}]" @click="getactive(1)">
        <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M8.70806 0.292786C8.52024 0.105315 8.26554 0 7.99997 0C7.7344 0 7.4797 0.105315 7.29188 0.292786L0.281113 7.29279C0.0986748 7.48139 -0.00227458 7.73399 7.34321e-06 7.99619C0.00228927 8.25838 0.10762 8.5092 0.293313 8.6946C0.479007 8.88001 0.730205 8.98518 0.992805 8.98746C1.2554 8.98974 1.5084 8.88894 1.69729 8.70679L1.99074 8.41379V14.9998C1.99074 15.265 2.09626 15.5194 2.28408 15.7069C2.47191 15.8944 2.72665 15.9998 2.99228 15.9998H4.99535C5.26098 15.9998 5.51572 15.8944 5.70355 15.7069C5.89137 15.5194 5.99689 15.265 5.99689 14.9998V12.9998C5.99689 12.7346 6.10241 12.4802 6.29024 12.2927C6.47806 12.1051 6.73281 11.9998 6.99843 11.9998H9.00151C9.26713 11.9998 9.52188 12.1051 9.7097 12.2927C9.89753 12.4802 10.003 12.7346 10.003 12.9998V14.9998C10.003 15.265 10.1086 15.5194 10.2964 15.7069C10.4842 15.8944 10.739 15.9998 11.0046 15.9998H13.0077C13.2733 15.9998 13.528 15.8944 13.7159 15.7069C13.9037 15.5194 14.0092 15.265 14.0092 14.9998V8.41379L14.3026 8.70679C14.4915 8.88894 14.7445 8.98974 15.0071 8.98746C15.2697 8.98518 15.5209 8.88001 15.7066 8.6946C15.8923 8.5092 15.9976 8.25838 15.9999 7.99619C16.0022 7.73399 15.9013 7.48139 15.7188 7.29279L8.70806 0.292786Z" :style="{fill: activeindex == 1 ? 'white' : '#C7C7D2'}"/>
        </svg>
      </div>
      <div :class="['mybutton', {active: activeindex == 2}]" @click="getactive(2)">
        <svg width="16" height="14" viewBox="0 0 16 14" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M13.1905 1H2.52379C1.68221 1 0.999969 1.59696 0.999969 2.33334V11.6667C0.999969 12.4031 1.68221 13.0001 2.52379 13.0001H13.1905C14.0321 13.0001 14.7143 12.4031 14.7143 11.6667V2.33334C14.7143 1.59696 14.0321 1 13.1905 1Z" :style="{stroke: activeindex == 2 ? 'white' : '#C7C7D2'}" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M0.999969 5.00114H14.7143" :style="{stroke: activeindex == 2 ? 'white' : '#C7C7D2'}" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M5.57114 13.0012V5.00114" :style="{stroke: activeindex == 2 ? 'white' : '#C7C7D2'}" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
      </div>
      <div :class="['mybutton', {active: activeindex == 3}]" @click="getactive(3)">
        <svg width="16" height="12" viewBox="0 0 16 12" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M15 7.50007H13.9738C13.5693 7.50007 13.2046 7.25634 13.0499 6.88256L12.0445 4.45407C11.9862 4.31354 11.8877 4.19485 11.7624 4.11393C11.637 4.03301 11.4908 3.99372 11.3432 4.00134C11.1957 4.00896 11.054 4.06312 10.937 4.15655C10.8201 4.24998 10.7335 4.37822 10.6889 4.52407L9.53855 8.29671C9.24572 9.25701 7.87869 9.23518 7.61668 8.26601L5.80052 1.54807C5.75842 1.3921 5.66871 1.25443 5.54479 1.15565C5.42088 1.05687 5.26942 1.00229 5.11307 1.00007C4.95647 0.99791 4.80341 1.0484 4.67686 1.14395C4.5503 1.23951 4.45707 1.37499 4.41114 1.53007L2.84997 6.78486C2.72392 7.20913 2.33398 7.50007 1.89138 7.50007H0.999969" :style="{stroke: activeindex == 3 ? 'white' : '#C7C7D2'}" stroke-width="2" stroke-linecap="round"/>
        </svg>
      </div>
      <div :class="['mybutton', {active: activeindex == 4}]" @click="getactive(4)">
        <svg width="16" height="20" viewBox="0 0 16 20" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M7.99997 20C11.976 20 16 18.626 16 16V4C16 1.374 11.976 0 7.99997 0C4.02397 0 -3.05176e-05 1.374 -3.05176e-05 4V16C-3.05176e-05 18.626 4.02397 20 7.99997 20ZM7.99997 18C4.27797 18 1.99997 16.705 1.99997 16V14.732C3.54097 15.57 5.77697 16 7.99997 16C10.223 16 12.459 15.57 14 14.732V16C14 16.705 11.722 18 7.99997 18ZM7.99997 2C11.722 2 14 3.295 14 4C14 4.705 11.722 6 7.99997 6C4.27797 6 1.99997 4.705 1.99997 4C1.99997 3.295 4.27797 2 7.99997 2ZM1.99997 6.732C3.54097 7.57 5.77697 8 7.99997 8C10.223 8 12.459 7.57 14 6.732V8C14 8.705 11.722 10 7.99997 10C4.27797 10 1.99997 8.705 1.99997 8V6.732ZM1.99997 10.732C3.54097 11.57 5.77697 12 7.99997 12C10.223 12 12.459 11.57 14 10.732V12C14 12.705 11.722 14 7.99997 14C4.27797 14 1.99997 12.705 1.99997 12V10.732Z" :style="{fill: activeindex == 4 ? 'white' : '#C7C7D2'}"/>
        </svg>
      </div>
      <div :class="['mybutton', {active: activeindex == 5}]" @click="getactive(5)">
        <svg width="16" height="14" viewBox="0 0 16 14" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M14.5459 0H4.36435C3.9786 0 3.60864 0.163889 3.33587 0.455612C3.06309 0.747335 2.90985 1.143 2.90985 1.55556V3.11111H4.36435V1.55556H14.5459V9.33333H13.0914V10.8889H14.5459C14.9316 10.8889 15.3016 10.725 15.5744 10.4333C15.8471 10.1416 16.0004 9.74589 16.0004 9.33333V1.55556C16.0004 1.143 15.8471 0.747335 15.5744 0.455612C15.3016 0.163889 14.9316 0 14.5459 0Z" :style="{fill: activeindex == 5 ? 'white' : '#C7C7D2'}"/>
          <path d="M11.636 3.11035H1.45447C1.06871 3.11035 0.698756 3.27424 0.425983 3.56596C0.153211 3.85769 -3.05176e-05 4.25335 -3.05176e-05 4.66591V12.4437C-3.05176e-05 12.8562 0.153211 13.2519 0.425983 13.5436C0.698756 13.8354 1.06871 13.9992 1.45447 13.9992H11.636C12.0218 13.9992 12.3917 13.8354 12.6645 13.5436C12.9373 13.2519 13.0905 12.8562 13.0905 12.4437V4.66591C13.0905 4.25335 12.9373 3.85769 12.6645 3.56596C12.3917 3.27424 12.0218 3.11035 11.636 3.11035ZM1.45447 12.4437V4.66591H11.636V12.4437H1.45447Z" :style="{fill: activeindex == 5 ? 'white' : '#C7C7D2'}"/>
        </svg>
      </div>
      <div :class="['mybutton', {active: activeindex == 6}]" @click="getactive(6)">
        <svg width="16" height="12" viewBox="0 0 16 12" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M13.6 0H2.39997C1.76345 0 1.153 0.237053 0.702913 0.65901C0.252826 1.08097 -3.05176e-05 1.65326 -3.05176e-05 2.25V9.75C-3.05176e-05 10.3467 0.252826 10.919 0.702913 11.341C1.153 11.7629 1.76345 12 2.39997 12H13.6C14.2365 12 14.8469 11.7629 15.297 11.341C15.7471 10.919 16 10.3467 16 9.75V2.25C16 1.65326 15.7471 1.08097 15.297 0.65901C14.8469 0.237053 14.2365 0 13.6 0ZM13.064 1.5L7.99997 5.0625L2.93597 1.5H13.064ZM13.6 10.5H2.39997C2.1878 10.5 1.98431 10.421 1.83428 10.2803C1.68426 10.1397 1.59997 9.94891 1.59997 9.75V2.4375L7.51997 6.6C7.65845 6.69737 7.82687 6.75 7.99997 6.75C8.17307 6.75 8.34149 6.69737 8.47997 6.6L14.4 2.4375V9.75C14.4 9.94891 14.3157 10.1397 14.1657 10.2803C14.0156 10.421 13.8121 10.5 13.6 10.5Z" :style="{fill: activeindex == 6 ? 'white' : '#C7C7D2'}"/>
        </svg>
      </div>
      <div :class="['mybutton', {active: activeindex == 7}]" @click="getactive(7)">
        <svg width="16" height="14" viewBox="0 0 16 14" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M11.4996 10.9522C10.4181 10.9522 9.22632 11.3668 8.13869 11.9017C6.39044 12.7618 5.51632 13.1922 5.08582 12.9177C4.65532 12.644 4.73669 11.7939 4.90032 10.0946L4.93707 9.70816" :style="{stroke: activeindex == 7 ? 'white' : '#C7C7D2'}" stroke-width="2" stroke-linecap="round"/>
          <path d="M11.5 9.95198C10.9477 9.95198 10.5 10.3997 10.5 10.952C10.5 11.5043 10.9477 11.952 11.5 11.952V9.95198ZM2.99997 2H13V0H2.99997V2ZM14 3V8.95198H16V3H14ZM1.99997 8.95198V3H-3.05176e-05V8.95198H1.99997ZM13 9.95198H11.5V11.952H13V9.95198ZM4.49997 9.95198H2.99997V11.952H4.49997V9.95198ZM-3.05176e-05 8.95198C-3.05176e-05 10.6088 1.34312 11.952 2.99997 11.952V9.95198C2.44768 9.95198 1.99997 9.50426 1.99997 8.95198H-3.05176e-05ZM14 8.95198C14 9.50426 13.5523 9.95198 13 9.95198V11.952C14.6568 11.952 16 10.6088 16 8.95198H14ZM13 2C13.5523 2 14 2.44772 14 3H16C16 1.34315 14.6568 0 13 0V2ZM2.99997 0C1.34311 0 -3.05176e-05 1.34315 -3.05176e-05 3H1.99997C1.99997 2.44772 2.44769 2 2.99997 2V0Z" :style="{fill: activeindex == 7 ? 'white' : '#C7C7D2'}"/>
        </svg>
      </div>
      <div :class="['mybutton', {active: activeindex == 8}]" @click="getactive(8)">
        <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M15.7646 3.55609C15.6218 3.28997 15.4174 3.06821 15.1712 2.91242C14.925 2.75663 14.6455 2.67215 14.36 2.6672H3.78413L3.30492 0.658302C3.2565 0.464379 3.14848 0.293806 2.99845 0.174364C2.84841 0.0549213 2.66521 -0.0063527 2.47868 0.000521318H0.826206C0.607075 0.000521318 0.396918 0.0941722 0.241969 0.260872C0.0870191 0.427572 -3.05176e-05 0.653665 -3.05176e-05 0.889414C-3.05176e-05 1.12516 0.0870191 1.35126 0.241969 1.51796C0.396918 1.68466 0.607075 1.77831 0.826206 1.77831H1.85074L4.13115 10.8983C4.17957 11.0923 4.28759 11.2628 4.43762 11.3823C4.58766 11.5017 4.77086 11.563 4.95739 11.5561H12.3935C12.5461 11.5556 12.6956 11.5097 12.8254 11.4234C12.9552 11.3371 13.0602 11.2138 13.1289 11.0672L15.8389 5.2361C15.9564 4.97122 16.0111 4.67918 15.9981 4.38604C15.9851 4.09289 15.9049 3.80776 15.7646 3.55609ZM11.8813 9.77834H5.58533L4.23856 4.44498H14.36L11.8813 9.77834Z" :style="{fill: activeindex == 8 ? 'white' : '#C7C7D2'}"/>
          <path d="M4.54355 16.0007C5.22803 16.0007 5.78291 15.4037 5.78291 14.6673C5.78291 13.9309 5.22803 13.334 4.54355 13.334C3.85908 13.334 3.3042 13.9309 3.3042 14.6673C3.3042 15.4037 3.85908 16.0007 4.54355 16.0007Z" :style="{fill: activeindex == 8 ? 'white' : '#C7C7D2'}"/>
          <path d="M12.8064 16.0007C13.4909 16.0007 14.0458 15.4037 14.0458 14.6673C14.0458 13.9309 13.4909 13.334 12.8064 13.334C12.122 13.334 11.5671 13.9309 11.5671 14.6673C11.5671 15.4037 12.122 16.0007 12.8064 16.0007Z" :style="{fill: activeindex == 8 ? 'white' : '#C7C7D2'}"/>
        </svg>
      </div>
      <div :class="['mybutton', {active: activeindex == 9}]" @click="getactive(9)">
        <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M7.99997 16C5.78753 16 3.87997 15.2089 2.33241 13.648C0.784858 12.0916 -3.05176e-05 10.1911 -3.05176e-05 8C-3.05176e-05 5.78844 0.785747 3.88089 2.33508 2.33333C3.88175 0.785778 5.78841 0 7.99997 0C10.192 0 12.0924 0.784889 13.648 2.33244C15.208 3.88089 16 5.78844 16 8C16 10.1911 15.2089 12.0924 13.6497 13.6507C12.0933 15.2089 10.1929 16 7.99997 16ZM7.99997 1.77778C6.25241 1.77778 4.81064 2.37067 3.59286 3.59111C2.37153 4.81067 1.77775 6.25244 1.77775 8C1.77775 9.728 2.37153 11.1662 3.59375 12.3956C4.8133 13.6249 6.25419 14.2222 7.99997 14.2222C9.72708 14.2222 11.1644 13.624 12.392 12.3938C13.624 11.1636 14.2222 9.72533 14.2222 8C14.2222 6.25511 13.6249 4.81333 12.3955 3.59378C11.1662 2.37156 9.72886 1.77778 7.99997 1.77778ZM5.3333 10.2222C4.10753 10.2222 3.11108 9.22578 3.11108 8C3.11108 6.77422 4.10753 5.77778 5.3333 5.77778C6.55908 5.77778 7.55553 6.77422 7.55553 8C7.55553 9.22578 6.55908 10.2222 5.3333 10.2222ZM5.3333 6.66667C4.59819 6.66667 3.99997 7.26489 3.99997 8C3.99997 8.73511 4.59819 9.33333 5.3333 9.33333C6.06841 9.33333 6.66664 8.73511 6.66664 8C6.66664 7.26489 6.06841 6.66667 5.3333 6.66667ZM10.6666 10.2222C9.44086 10.2222 8.44441 9.22578 8.44441 8C8.44441 6.77422 9.44086 5.77778 10.6666 5.77778C11.8924 5.77778 12.8889 6.77422 12.8889 8C12.8889 9.22578 11.8924 10.2222 10.6666 10.2222Z" :style="{fill: activeindex == 9 ? 'white' : '#C7C7D2'}"/>
        </svg>
      </div>
      <div :class="['mybutton', {active: activeindex == 10}]" @click="getactive(10)">
        <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M7.99997 16C5.78753 16 3.87997 15.2089 2.33241 13.648C0.784858 12.0916 -3.05176e-05 10.1911 -3.05176e-05 8C-3.05176e-05 5.78844 0.785747 3.88089 2.33508 2.33333C3.88175 0.785778 5.78841 0 7.99997 0C10.192 0 12.0924 0.784889 13.648 2.33244C15.208 3.88089 16 5.78844 16 8C16 10.1911 15.2089 12.0924 13.6497 13.6507C12.0933 15.2089 10.1929 16 7.99997 16ZM7.99997 1.77778C6.25241 1.77778 4.81064 2.37067 3.59286 3.59111C2.37153 4.81067 1.77775 6.25244 1.77775 8C1.77775 9.728 2.37153 11.1662 3.59375 12.3956C4.8133 13.6249 6.25419 14.2222 7.99997 14.2222C9.72708 14.2222 11.1644 13.624 12.392 12.3938C13.624 11.1636 14.2222 9.72533 14.2222 8C14.2222 6.25511 13.6249 4.81333 12.3955 3.59378C11.1662 2.37156 9.72886 1.77778 7.99997 1.77778Z" :style="{fill: activeindex == 10 ? 'white' : '#C7C7D2'}"/>
          <circle cx="7.99997" cy="8" r="3" :style="{stroke: activeindex == 10 ? 'white' : '#C7C7D2'}" stroke-width="2"/>
        </svg>
      </div>
      <div :class="['mybutton', {active: activeindex == 11}]" @click="getactive(11)">
        <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M13.6 1.6H12V0.8C12 0.587827 11.9157 0.384344 11.7657 0.234315C11.6156 0.0842854 11.4121 0 11.2 0C10.9878 0 10.7843 0.0842854 10.6343 0.234315C10.4843 0.384344 10.4 0.587827 10.4 0.8V1.6H5.59997V0.8C5.59997 0.587827 5.51568 0.384344 5.36565 0.234315C5.21563 0.0842854 5.01214 0 4.79997 0C4.5878 0 4.38431 0.0842854 4.23428 0.234315C4.08426 0.384344 3.99997 0.587827 3.99997 0.8V1.6H2.39997C1.76345 1.6 1.153 1.85286 0.702913 2.30294C0.252826 2.75303 -3.05176e-05 3.36348 -3.05176e-05 4V13.6C-3.05176e-05 14.2365 0.252826 14.847 0.702913 15.2971C1.153 15.7471 1.76345 16 2.39997 16H13.6C14.2365 16 14.8469 15.7471 15.297 15.2971C15.7471 14.847 16 14.2365 16 13.6V4C16 3.36348 15.7471 2.75303 15.297 2.30294C14.8469 1.85286 14.2365 1.6 13.6 1.6ZM14.4 13.6C14.4 13.8122 14.3157 14.0157 14.1657 14.1657C14.0156 14.3157 13.8121 14.4 13.6 14.4H2.39997C2.1878 14.4 1.98431 14.3157 1.83428 14.1657C1.68426 14.0157 1.59997 13.8122 1.59997 13.6V8H14.4V13.6ZM14.4 6.4H1.59997V4C1.59997 3.78783 1.68426 3.58434 1.83428 3.43431C1.98431 3.28429 2.1878 3.2 2.39997 3.2H3.99997V4C3.99997 4.21217 4.08426 4.41566 4.23428 4.56569C4.38431 4.71571 4.5878 4.8 4.79997 4.8C5.01214 4.8 5.21563 4.71571 5.36565 4.56569C5.51568 4.41566 5.59997 4.21217 5.59997 4V3.2H10.4V4C10.4 4.21217 10.4843 4.41566 10.6343 4.56569C10.7843 4.71571 10.9878 4.8 11.2 4.8C11.4121 4.8 11.6156 4.71571 11.7657 4.56569C11.9157 4.41566 12 4.21217 12 4V3.2H13.6C13.8121 3.2 14.0156 3.28429 14.1657 3.43431C14.3157 3.58434 14.4 3.78783 14.4 4V6.4Z" :style="{fill: activeindex == 11 ? 'white' : '#C7C7D2'}"/>
        </svg>
      </div>
    </div>
  </div>
  <div class="withinput">
    <div class="firstcontainer">
      <div class="inp">
        <button><img src="@/assets/msearch.svg" alt="search"></button>
        <input type="text" placeholder="Search Anything">
      </div>
      <div class="person">
        <div @click="chatting">
          <svg width="16" height="12" viewBox="0 0 16 12" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M13.6004 0H2.40037C1.76385 0 1.1534 0.237053 0.70331 0.65901C0.253223 1.08097 0.000366211 1.65326 0.000366211 2.25V9.75C0.000366211 10.3467 0.253223 10.919 0.70331 11.341C1.1534 11.7629 1.76385 12 2.40037 12H13.6004C14.2369 12 14.8473 11.7629 15.2974 11.341C15.7475 10.919 16.0004 10.3467 16.0004 9.75V2.25C16.0004 1.65326 15.7475 1.08097 15.2974 0.65901C14.8473 0.237053 14.2369 0 13.6004 0ZM13.0644 1.5L8.00037 5.0625L2.93637 1.5H13.0644ZM13.6004 10.5H2.40037C2.18819 10.5 1.98471 10.421 1.83468 10.2803C1.68465 10.1397 1.60037 9.94891 1.60037 9.75V2.4375L7.52037 6.6C7.65884 6.69737 7.82727 6.75 8.00037 6.75C8.17346 6.75 8.34189 6.69737 8.48037 6.6L14.4004 2.4375V9.75C14.4004 9.94891 14.3161 10.1397 14.1661 10.2803C14.016 10.421 13.8125 10.5 13.6004 10.5Z" fill="#4E4E4E"/>
          </svg>
        </div>
        <div @click="notification">
          <svg width="17" height="19" viewBox="0 0 17 19" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M10.0493 18.1273C10.0493 18.3587 9.96172 18.5807 9.80581 18.7444C9.64991 18.9081 9.43845 19 9.21797 19H4.78419C4.5637 19 4.35225 18.9081 4.19634 18.7444C4.04044 18.5807 3.95285 18.3587 3.95285 18.1273C3.95285 17.8958 4.04044 17.6738 4.19634 17.5102C4.35225 17.3465 4.5637 17.2545 4.78419 17.2545H9.21797C9.43845 17.2545 9.64991 17.3465 9.80581 17.5102C9.96172 17.6738 10.0493 17.8958 10.0493 18.1273ZM13.6739 15.3631C13.5538 15.5853 13.3794 15.7699 13.1687 15.8978C12.958 16.0258 12.7186 16.0924 12.4752 16.0909H1.52695C1.28352 16.0924 1.04412 16.0258 0.833402 15.8978C0.622686 15.7699 0.448282 15.5852 0.328162 15.363C0.206864 15.1408 0.143329 14.889 0.143925 14.6329C0.144521 14.3768 0.209226 14.1253 0.331556 13.9037C0.725748 13.1917 1.1958 11.8324 1.1958 9.4V9.10909C1.19396 7.49085 1.80453 5.93812 2.89319 4.79245C3.98186 3.64678 5.45945 3.00202 7.00094 3L7.04528 3.00015C10.2222 3.02495 12.8069 5.79491 12.8069 9.17484V9.4C12.8069 11.8326 13.2766 13.192 13.6707 13.904C13.793 14.1256 13.8576 14.377 13.8582 14.6331C13.8588 14.8891 13.7952 15.1409 13.6739 15.3631ZM12.0145 14.3455C11.3018 12.7782 11.1442 10.822 11.1442 9.4V9.17484C11.1442 6.75025 9.29993 4.7632 7.03295 4.7456C7.02239 4.74551 7.01184 4.74547 7.00129 4.74545C6.45633 4.74641 5.9169 4.86003 5.41377 5.07984C4.91065 5.29965 4.4537 5.62134 4.069 6.02654C3.6843 6.43175 3.3794 6.91252 3.1717 7.44143C2.96399 7.97033 2.85756 8.537 2.85847 9.10909V9.4C2.85847 10.822 2.70079 12.7783 1.98764 14.3455H12.0145Z" fill="#4E4E4E"/>
            <circle cx="12.0004" cy="5" r="5" fill="#563BFF"/>
            <path d="M10.4164 4.90234L10.6625 2.73438H13.0531V3.44043H11.3568L11.2513 4.35742C11.4525 4.25 11.6664 4.19629 11.8929 4.19629C12.2992 4.19629 12.6176 4.32227 12.848 4.57422C13.0785 4.82617 13.1937 5.17871 13.1937 5.63184C13.1937 5.90723 13.1351 6.1543 13.0179 6.37305C12.9027 6.58984 12.7367 6.75879 12.5199 6.87988C12.3031 6.99902 12.0472 7.05859 11.7523 7.05859C11.4945 7.05859 11.2552 7.00684 11.0345 6.90332C10.8138 6.79785 10.639 6.65039 10.5101 6.46094C10.3832 6.27148 10.3158 6.05566 10.308 5.81348H11.1459C11.1635 5.99121 11.225 6.12988 11.3304 6.22949C11.4379 6.32715 11.5775 6.37598 11.7494 6.37598C11.9408 6.37598 12.0883 6.30762 12.1918 6.1709C12.2953 6.03223 12.347 5.83691 12.347 5.58496C12.347 5.34277 12.2875 5.15723 12.1683 5.02832C12.0492 4.89941 11.8802 4.83496 11.6615 4.83496C11.4603 4.83496 11.2972 4.8877 11.1722 4.99316L11.0902 5.06934L10.4164 4.90234Z" fill="white"/>
          </svg>
        </div>
        <div class="profile" @click="profile">
          <img src="@/assets/myprof.jpg" alt="profile">
        </div>
      </div>
    </div>
    <div class="nextline">
      <div class="first">
        <div class="graph">
          <h3>Performance </h3>
          <img src="@/assets/real.png" alt="vector">
          <div class="mymonth">
            <h5 v-for="(month, index) in monthes" :key="index" :class="['default', { add : month == currentmonth}]">{{ month }}</h5>
          </div>
        </div>
        
        <div class="yana">
          <h3 class="ortiq">Session By Device</h3>
          <div class="box">
            
            <div class="semi">
              <div :style="divstyle(bir, '#A93BFF', '75')">
                <svg>
                  <circle :cx="bir" :cy="bir" :r="bir"></circle>
                  <circle :cx="bir" :cy="bir" :r="bir"></circle>
                </svg>
              </div>
              <div :style="divstyle(ikki, '#FF7049', '50')" >
                <svg>
                  <circle :cx="ikki" :cy="ikki" :r="ikki"></circle>
                  <circle :cx="ikki" :cy="ikki" :r="ikki"></circle>
                </svg>
              </div>
              <div :style="divstyle(uch, '#20C997', '25')" >
                <svg>
                  <circle :cx="uch" :cy="uch" :r="uch"></circle>
                  <circle :cx="uch" :cy="uch" :r="uch"></circle>
                </svg>
              </div>
            </div>
            <div class="info">
              <div>
                <p>Desktop</p>
                <h3>8,085 <span>13%</span></h3>
              </div>
              <div>
                <p>Mobile</p>
                <h3>8,085 <span>30%</span></h3>
              </div>
              <div>
                <p>Tablets</p>
                <h3>8,085 <span>25%</span></h3>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="anotherline">
      <div class="sina">
        <div>
          <div class="data">
            <div class="users">
              <div><img src="@/assets/bir.svg" alt="users"></div>
              <p>Users</p>
              <h3>72.6k</h3>
              <h5>+25%</h5>
            </div>
            <div class="users">
              <div><img src="@/assets/ikki.svg" alt="sessions"></div>
              <p>Sessions</p>
              <h3>87.2k</h3>
              <h5>+47%</h5>
            </div>
            <div class="users">
              <div><img src="@/assets/uch.svg" alt="bounce"></div>
              <p>Bounce Rate</p>
              <h3>26.3%</h3>
              <h5>-28%</h5>
            </div>
            <div class="users">
              <div><img src="@/assets/tort.svg" alt="duration"></div>
              <p>Session Duration</p>
              <h3>2m 18s</h3>
              <h5>+13%</h5>
            </div>
          </div>
          <div class="inn">
            <p>Daily Overview</p>
            <button>Export</button>
          </div>
        </div>
      </div>
      <div class="device">
        <div>
          <h2>Session By Device</h2>
          <div class="channel">
            <p class="forp">Channel</p>
            <p class="myrange">Traffic (%)</p>
            <p class="anotherp">Value</p>
          </div>
        </div>
        <hr>
        <div :style="last('rgb(86,59,255)', '148px')" class="fdir">
          <p class="forp"> Direct</p>
          <div>
            <div></div>
            <div></div>
          </div>
          <p class="anotherp">23.28%</p>
        </div>
        <div :style="last('rgb(255, 112,73)', '176px')" class="fdir">
          <p class="forp">Direct</p>
          <div>
            <div></div>
            <div></div>
          </div>
          <p class="anotherp">23.28%</p>
        </div>
        <div :style="last('rgb(32,201,151)', '113px')" class="fdir">
          <p class="forp">Direct</p>
          <div>
            <div></div>
            <div></div>
          </div>
          <p class="anotherp">23.28%</p>
        </div>
        
      </div>

        
    </div>
    <div class="otherline">
      <div class="mine">
        <div class="anot">
          <div class="one">
            <div>
              <p>5,461</p>
              <h5>Today</h5>
            </div>
            <div :style="divstylem('rgb(86, 59, 255)')" class="foruser">
              <p>Users</p>
              <svg>
                <circle cx="30" cy="30" r="30"></circle>
                <circle cx="30" cy="30" r="30"></circle>
              </svg>
            </div>
            <div>
              <p>140</p>
              <h5>Today</h5>
            </div>
          </div>
          <div class="one">
            <div>
              <p>5,461</p>
              <h5>Today</h5>
            </div>
            <div :style="divstylem('rgb(255,112,73)')" class="foruser">
              <p>Goals</p>
              <svg>
                <circle cx="30" cy="30" r="30"></circle>
                <circle cx="30" cy="30" r="30"></circle>
              </svg>
            </div>
            <div>
              <p>120</p>
              <h5>Expected</h5>
            </div>
          </div>
        </div>
      </div>
      <div class="mylast">
          <div>
            <h4>Session By Device</h4>
            <p>Top region & Session</p>
          </div>
          <button>View</button>
      </div>

    </div>
  </div>
</div>

</template>
<script>
  export default{
    data(){
      return{
        currentmonth : "",
        bir: 86,
        ikki: 50,
        uch: 20,
        monthes: ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
        activeindex: 1,
      }
    },
    created(){
      this.getmonth();
    },
    methods:{
      last(mycol, uzunlik){
        return{
          '--mycol' : mycol,
          '--uzunlik': uzunlik,
        }
      },
      divstylem(col){
        return{
          '--ncolor': col
        }
        
      },
      divstyle(mylength, mycolor, mypercent){
        return{
          '--len': mylength + 'px',
          '--mycolor': mycolor,
          '--percent': mypercent,
          '--circum' : mylength * 6.28,
        }
      },
      getmonth(){
        const date = new Date();
        const month = date.toLocaleString('default', { month: 'long' });
        this.currentmonth = month.slice(0, 3);
      },
      getactive(index){
        this.activeindex = index;
      },
      notification(){
        // Bu yangi xabarlar qismi
      },
      chatting(){
        // Bu chat page uchun
      },
      profile(){
        // Bu profile page uchun
      }
    }
  }
</script>
<style scoped>
.otherline{
  display: flex;
  width: 100%;
  gap: 10px 30px;
  justify-content: space-between;
  flex-wrap: wrap;
  margin-top: 10px;
}
.mylast{
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-basis: 200px;
  flex-shrink: 2;
  flex-grow: 2;
  background-color: white;
  border-radius: 10px;
  box-shadow: 0 0  7px rgb(203, 200, 200);
  margin-top: 5px
};

.mylast h4{
  transform: translateX(10px);
}
.mylast button{
  margin-right: 15px;
}
.myrange{
  width: 250px;
}
.fdir>div div:nth-child(1){
  width: 230px;
  height: 5px;
  background-color: #F2F3F9;
  border-radius: 7px;
}
.fdir >div{
  left: 10px;
}
.fdir>div div:nth-child(2){
  position: absolute;
  width: var(--uzunlik);
  height: 5px;
  background-color: var(--mycol);
  border-radius: 7px;
  transform: translateY(-5px);
}
.fdir{
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: -7px;
}
.inn button{
  color: white;
  padding: 7px 30px;
  border-radius: 8px;
  background-color: rgba(169, 59, 255, 1);
  border: none;
}
.device>div > h2{
  margin-left: 10px;
}
.mylast button{
  color: white;
  padding: 7px 30px;
  border-radius: 8px;
  background-color: rgba(169, 59, 255, 1);
  border: none;
}
.device{
  width: 650px;
  flex: 2;
  background-color: white;
  border-radius: 10px;
  box-shadow: 0 0  7px rgb(203, 200, 200);
  height: min-content;
  margin-top: 10px;
}
.channel{
  display: flex;
  justify-content: space-between;
  margin-top: -15px;
}
.anotherline{
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 0 30px;
  width: 100%;
  margin-top: 10px;
}
.anot{
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 650px;
  gap: 0 30px;
  height: initial;
}
.one{
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-shrink: 1;
  flex-grow: 1;
  flex-basis: 200px;
  width: 160px;
  background-color: white;
  border-radius: 10px;
  box-shadow: 0 0 7px rgb(203, 200, 200);

}
.one >div:nth-child(1) >p{
  margin-left: 10px;
}
.one>div:nth-child(1) h5{
  margin-left: 10px;
}
.one>div:nth-child(3) h5{
  margin-right: 10px;
}
.inn{
  width: 650px;
  display: flex;
  flex: 1.5;
  justify-content: space-between;
  align-items: center;
}
.inn p{
  margin-left: 10px;
}
.inn button{
  margin-right: 15px;
}
.foruser{
  width: 66px;
  height: 66px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.foruser p{
  display: absolute;
  color: var(--ncolor);
  font-weight: 700;
  font-size: 15px;
}
.foruser svg{
  width: 66px;
  height: 66px;
  position: absolute;
}
.foruser svg circle{
  fill: none;
  stroke: var(--ncolor);
  stroke-width: 6;
  transform: translate(3px, 3px);
  stroke-dashoffset: 47;
  stroke-dasharray: 188;
  stroke-linecap: round;
}
.foruser svg circle:nth-child(1){
  stroke: #F2F3F9;
  stroke-dashoffset: 0;
}
.users:nth-child(1) div{
  background-color: rgba(53, 117, 255, 0.1);
}
.users:nth-child(2) div{
  background: rgba(243, 102, 67, .1);

}
.users:nth-child(3) div{
  background: rgba(69, 36, 248, .1);

}
.users:nth-child(4) div{
  background: rgba(36, 214, 165, .1);

}
.users p{
  font-weight: 700;
  font-size: 14px;
  line-height: 16px;
  color: rgba(90, 88, 129);
}
.users h5{
  font-weight: 500;
  font-size: 14px;
  line-height: 16px;
  color: rgba(90, 88, 129);
  margin-top: -20px;
}
.users h3{
  font-weight: 500;
  font-size: 24px;
  line-height: 28px;
  color: rgba(21, 19, 75);
  margin-top: -10px;
}
.users{
  flex-grow: 1;
  flex-shrink: 1;
  flex-basis: 120px;
  width: 120px !important;
  background-color: white;
  border-radius: 7px;
  box-shadow: 0 0 7px rgb(203, 200, 200);
}
.users div{
  padding: 10px;
  height: max-content;
  width: max-content;
  border-radius: 10px;
}
.data{
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 0 30px;
}
.data > div{
  width: 120px;
  height: max-content;
  padding: 20px 0 0 20px;
}
.info span{
  color: #5A5881;
  font-size: 13px;
  line-height: 15px;
  font-weight: 500;
}
.info p{
  color: #5A5881;
  font-size: 14px;
  line-height: 16px;
  font-weight: 700;
}
.info h3{
  margin-top: -3px;
  color: #15134B;
  font-size: 18px;
  line-height: 21px;
  font-weight: 500;
}
.ortiq{
  top: 0;
  position: relative;
}
.yana{
  width: 510px;
  flex: 1;
  background-color: white;
  border-radius: 10px;
  box-shadow: 0 0 7px rgb(203, 200, 200);
}
.sina{
  flex: 1.5;
  width: 650px;
  border-radius: 10px;
}
.box{
  display: flex;
  justify-content: space-around;
  align-items: center;
}
*{
  font-family: 'Roboto';
}
.first{
  display: flex;
  justify-content: space-between;
  gap: 10px 30px;
  flex-wrap: wrap;
  margin-top: 10px;
}
.semi div{
  position: absolute;
}
.semi{
  width: 190px;
  height: initial;
  display: flex;
  justify-content: center;
  align-items: center;
}
.semi svg{
  width: calc(var(--len) * 2 + 10px);
  height: calc(var(--len) * 2 + 10px);
  transform: rotate( -90deg);
}
.semi svg circle{
  fill: none;
  stroke-width: 10;
  transform: translate(5px, 5px);
  stroke-dasharray: var(--circum);
  stroke-dashoffset: var(--circum);
  stroke-linecap: round;
}
.semi svg circle:nth-child(1){
  stroke: #F2F3F9;
  stroke-dashoffset: 0;
}
.semi svg circle:nth-child(2){
  stroke: var(--mycolor);
  stroke-dashoffset: calc(var(--circum) - (var(--percent) * var(--circum))/100);
}
.mymonth{
  margin: auto;
  width: 592px;
  display: flex;
  justify-content: space-between;
}
.graph  img{
  width: 600px;
  /* width: clamp(350px, 40vw, 700px); */
  margin: auto;
}
.graph{
  max-width: 650px;
  flex: 1.5;
  display: flex;
  flex-wrap: wrap;
  background-color: white;
  border-radius: 10px;
  box-shadow: 0 0 7px rgb(203, 200, 200);
}
.default{
  color: #A3ABBD;
  font-weight: 500;
  font-family: Poppins;
  font-size: 12px;
  line-height: 18px;
}
.add{
  color: #4E4E4E;
}
.person{
  width: 80px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-right: 15px;
}
.profile >img{
  width: 20px;
  height: 20px;
  border-radius: 50%;
}
.inp{
  margin-left: 20px;
}
.firstcontainer{
  display: flex;
  height: 80px;
  justify-content: space-between;
  align-items: center;
  background-color: white;
}
.withinput{
  width: calc(100% - 150px);
  margin: 0 20px;
}
.inp button{
  transform: translateY(2px);
  width: 13px;
  height: 13px;
  padding: 0;
  border: none;
  background: transparent;
}
.inp button > img{
  width: 100%;
  object-fit: contain;
}
input{
  border: none;
  font-weight: 300;
  color: #5A5881;
  margin-left: 3px;
  width: 100px;
}
.logo{
  height: 20%;
  display: flex;
  justify-content: center;
}
.logo > svg{
  margin: 44px auto;
}
.buttons{
  margin-bottom: 0;
  display: flex;
  justify-content: center;
  flex-direction: column;
  height: 80%;
  width: initial;
}
.mybutton{
  width: 66px;
  height: 48px;
  cursor: pointer;
  border-radius: 15px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: auto auto;
}
.active::before{
  content: "";
  position: absolute;
  width: 3px;
  height: 35px;
  left: 0;
  border-top-right-radius: 4px;
  border-bottom-right-radius: 4px;
  background-color: #3734A9;
}
.active > svg{
  width: 1.1em;
  animation: animate 0.2s linear;
  animation-iteration-count: 1;
}
@keyframes animate{
  0%{
    transform: rotate(-15deg);
  }
  50%{
    transform: rotate(15deg);
  }
  100%{
    transform: rotate(0);
  }
}
.mainconatiner{
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  min-height: 100vh;
  background-color: rgb(248, 248, 248);
}
.bars{
  width: 102px;
  height: initial;
  background-color: #ffffff;
}
.forp{
  margin-left: 12px;
}
.anotherp{
  margin-right: 12px;
}
.mine{
  width: 650px;
  flex: 1.5;
}
.active{
  background-color: #563bFF;
}
@media(max-width: 1164px){
  .graph img, .graph .mymonth{
    width: 45vw;
  }
}
@media(max-width: 1010px){
  .graph img, .graph .mymonth{
    width: 44vw;
  }
  .inn > button{
    margin-right: 40px;
  }
}
@media(max-width: 930px){
  .graph img, .graph .mymonth{
    width: 64vw;
  }
  .logo{
    height: 10%;
  }
}
@media (max-width: 910px){
  .semi{
    margin-left: -7vw;
  }
}
@media (max-width: 540px){
  .semi{
    margin-left: -2vw;
  }
}
@media (max-width: 1215px){
  .inn{
    width: 84vw;
  }
}
@media (max-width: 700px){
  .inn button{
    margin-right: 90px;
  }
  
}
@media(max-width: 850px){
  .graph img, .graph .mymonth{
    width: 70vw;
  }
  .inn  button{
    margin-right: 60px;
  }
}
@media(max-width: 590px){
  .graph img, .graph .mymonth{
    width: 66vw;
  }
}
@media (max-width:1263){
  .inn{
    width: 600px;
  }
}
@media (max-width: 815px){
  .users{
    flex-basis: 200px;
  }
}
@media (max-width: 1040px){
  .anot{
    width: 100%;
  }
}
</style>