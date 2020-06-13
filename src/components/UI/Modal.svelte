<style>

.modal-content {
    position: relative;
    display: -ms-flexbox;
    display: flex;
    -ms-flex-direction: column;
    flex-direction: column;
    width: 100%;
    pointer-events: auto;
    background-clip: padding-box;
    border: 1px solid rgba(0,0,0,.2);
    outline: 0;
    box-shadow: none;
    background-color: rgb(255, 255, 255);
    padding: 0px;
    border-radius: 20px;
}
.padding-top{
  padding-top: 6em;
}
.modal-header{
    border-bottom: none;
}
.modal-footer{
    border-top: none;
}
</style>
<script>
  import { createEventDispatcher } from "svelte";
  import {fade,fly} from 'svelte/transition'
//   import Button from "./Button.svelte";
  export let title;
  const dispatch = createEventDispatcher();
  function closeModal() {
    dispatch("cancel");
  }
</script>



<div class="modal fade padding-top" id="exampleModalLong" tabindex="-1" role="dialog" aria-labelledby="exampleModalLongTitle" aria-hidden="true">
  <div class="modal-dialog" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
          <slot />
      </div>
      <!-- <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Save changes</button>
      </div> -->
    </div>
  </div>
</div>
