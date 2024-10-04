<template>

  <!-- flex-shrink: 0とflex-shrink: 1が混在しているのでflex-shrink: 0は全く縮まない -->
  <div class="flex">
    <div class="columns">
      dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 .
    </div>
    <div class="divider"></div>
    <div class="columns">
      dummy2 ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
    </div>
  </div>
  
  </template>
  <style scoped>
  .flex {
    display: flex;
    flex-direction: row;
    margin-left: auto;
    margin-right: auto;
  }
  
  .columns {
    flex-shrink: 1;
  }
  
  .divider {
    flex-shrink: 0;
    width: 20px;
    background-color: black;
  }
  
  .columns-shrink0 {
    /* flex-shrink: 0にすると、そのflexアイテムではテキストの改行（wrap）が起きなくなる*/
    flex-shrink: 0;
  }
  </style>
  