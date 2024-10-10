<template>

<!-- 均等にする -->
<div class="flex">
  <div class="columns text-center">
    dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 dummy1 .
  </div>
  <div class="divider"></div>
  <div class="columns text-center">
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
  /* すべてのflexアイテムの flex-grow 係数が同じであれば、余白はすべてのアイテムに均等に分配されます。このような場合、ふつうは値に 1 を使用します */
  flex-grow: 1;
  /* flexアイテムの寸法を完全に無視したい場合は、 flex-basis を 0 に設定 */
  flex-basis: 0;
}

.text-center {
  text-align: center;
}

.divider {
  /* このflexアイテムは伸長収縮させない、width値をそのまま使う */
  /* flex-growのデフォルトは0なので、flex-grow: 0;は必要ないが一応入れてある */
  flex-grow: 0;
  flex-shrink: 0;
  width: 20px;
  background-color: black;
}

</style>
