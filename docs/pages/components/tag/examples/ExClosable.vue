<template>
    <section>
        <div class="field">
            <b-tag v-if="isTag1Active"
                type="is-primary"
                closable
                @close="isTag1Active = false">
                Colored closable tag label
            </b-tag>
        </div>

        <div class="field">
            <b-tag v-if="isTag2Active"
                attached
                closable
                @close="isTag2Active = false">
                Attached closable tag label
            </b-tag>
        </div>

        <div class="field">
            <b-tag v-if="isTag3Active"
                type="is-danger"
                attached
                closable
                @close="isTag3Active = false">
                Colored attached closable tag label
            </b-tag>
        </div>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                isTag1Active: true,
                isTag2Active: true,
                isTag3Active: true
            }
        }
    }
</script>
