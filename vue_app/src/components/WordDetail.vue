<script>
export default {
    props: {
        selectedWordData: Object
    }
};
</script>
<template>
    <!-- ///////////////////////////////////////////////////////////////////////////////////////////////
    //
    // ワードの詳細情報の表示
    //
    //////////////////////////////////////////////////////////////////////////////////////////////// -->
    <div>
        <div class="is-size-6">{{ selectedWordData.wordName }} とは？</div>
        <div class="is-size-7">{{ selectedWordData.explanation }} </div>
        <div class="is-size-7"><strong>タイプ:</strong> {{ selectedWordData.typeName }}</div>
    </div>
    <div>
        <a href="#" @click="$emit('closeWordDetailEvent')">元に戻す</a>
    </div>
</template>
