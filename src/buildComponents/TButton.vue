<template>
  <div class="Tbutton-container">
    BUTTON
  <div>{{idProp}}</div>
  </div>
</template>

<script lang='ts'>
import Vue from 'vue';
import Component, { mixins } from 'vue-class-component';

const TButtonProps = Vue.extend({
  props: {
    idProp: Number,
  },
});

@Component
export default class TButton extends TButtonProps {
  get id() {
    return this.idProp;
  }
}
</script>

<style>
.Tbutton-container {
  height: 100%;
  width: 100%;
  display: inline-block;
  margin-bottom: 0;
  font-weight: 400;
  text-align: center;
  vertical-align: middle;
  -ms-touch-action: manipulation;
  touch-action: manipulation;
  cursor: pointer;
  background-image: none;
  border: 1px solid transparent;
  white-space: nowrap;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  height: 32px;
  padding: 0 15px;
  font-size: 14px;
  border-radius: 4px;
  transition: color 0.2s linear, background-color 0.2s linear,
    border 0.2s linear, box-shadow 0.2s linear;
  color: #515a6e;
  background-color: #fff;
  border-color: #dcdee2;
}
</style>
