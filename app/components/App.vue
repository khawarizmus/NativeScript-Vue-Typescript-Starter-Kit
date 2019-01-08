<template>
    <Page>
        <ActionBar>
            <GridLayout width="100%" columns="auto, *">
                <Label text="MENU" @tap="$refs.drawer.nativeView.toggleDrawerState()" col="0"/>
                <Label class="title" text="Native-Vue-Typescript"  col="1"/>
            </GridLayout>
        </ActionBar>

        <RadSideDrawer ref="drawer">
            <StackLayout ~drawerContent backgroundColor="#ffffff">
                <Label class="drawer-header" text="Drawer"/>

                <Label class="drawer-item" text="Item 1"/>
                <Label class="drawer-item" text="Item 2"/>
                <Label class="drawer-item" text="Item 3"/>
            </StackLayout>

            <GridLayout ~mainContent columns="*" rows="*">
                <Label class="message" :text="msg" col="0" row="0"/>
            </GridLayout>
        </RadSideDrawer>
    </Page>
</template>

<script lang="ts">
import Vue from 'vue'
import Component from 'vue-class-component'

@Component
export default class App extends Vue {
    private msg = 'Hello {N}-vue + Typescript!'
}
</script>

<style scoped>
    ActionBar {
        background-color: #44B681;
        color: #2e2300;
    }

    .title {
        direction: rtl;
        text-align: center;
        padding-right: 16;
        font-size: 23%
    }

    .message {
        vertical-align: center;
        text-align: center;
        font-size: 20;
        color: #333333;
    }

    .drawer-header {
        padding: 50 16 16 16;
        margin-bottom: 16;
        background-color: #44B681;
        color: #2e2300;
        font-size: 24;
    }

    .drawer-item {
        padding: 8 16;
        color: #2e2300;
        font-size: 16;
    }
</style>
