<template>
  <div class="sets-list row">
    <div class="col-md-12">
      <div class="row">

        <div class="small-set col-lg-6">
          <vuestic-widget :headerText="$t('treeView.basic')">
            <tree-view-basic-preview/>
          </vuestic-widget>
        </div>

        <div class="small-set col-lg-6">
          <vuestic-widget :headerText="$t('treeView.icons')">
            <tree-view-icons-preview/>
          </vuestic-widget>
        </div>

        <div class="small-set col-lg-6">
          <vuestic-widget :headerText="$t('treeView.advanced')">
            <tree-view-advanced-preview/>
          </vuestic-widget>
        </div>


        <div class="small-set col-lg-6">
          <vuestic-widget :headerText="$t('treeView.editable')">
            <tree-view-editable-preview/>
          </vuestic-widget>
        </div>

        <div class="small-set col-lg-6">
          <vuestic-widget :headerText="$t('treeView.selectable')">
            <tree-view-selectable-preview/>
          </vuestic-widget>
        </div>

      </div>
    </div>
  </div>
</template>

<script>
  import VuesticWidget
    from '../../../vuestic-theme/vuestic-components/vuestic-widget/VuesticWidget.vue'
  import TreeViewBasicPreview from './TreeViewBasicPreview'
  import TreeViewIconsPreview from './TreeViewIconsPreview'
  import TreeViewSelectablePreview from './TreeViewSelectablePreview'
  import TreeViewAdvancedPreview from './TreeViewAdvancedPreview'
  import TreeViewEditablePreview from './TreeViewEditablePreview'

  export default {
    name: 'tree-view',
    components: {
      TreeViewEditablePreview,
      TreeViewAdvancedPreview,
      TreeViewSelectablePreview,
      TreeViewIconsPreview,
      TreeViewBasicPreview,
      VuesticWidget
    },
    data () {
      return {
        treeViewData: {}
      }
    }
  }
</script>

<style lang="scss">

</style>
