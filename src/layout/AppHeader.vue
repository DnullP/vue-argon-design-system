<template>
    <header class="header-global">
        <base-nav class="mt" type="primary" expand effect="dark">
            <router-link slot="brand" class="navbar-brand mr-lg-5" to="/">
                <img src="img/brand/white.png" alt="logo">
            </router-link>

            <div class="row" slot="content-header" slot-scope="{closeMenu}">
                <div class="col-6 collapse-brand">
                    <a href="https://demos.creative-tim.com/vue-argon-design-system/documentation/">
                        <img src="img/brand/blue.png">
                    </a>
                </div>
                <div class="col-6 collapse-close">
                    <close-button @click="closeMenu"></close-button>
                </div>
            </div>

            <ul class="navbar-nav navbar-nav-hover align-items-lg-center">
                <a slot="title" href="/#/" class="nav-link" role="button">
                    <i class="ni ni-ui-04 d-lg-none"></i>
                    <span class="nav-link-inner--text">公司首页</span>
                </a>
                <a slot="title" href="/#/Product" class="nav-link" role="button">
                    <i class="ni ni-ui-04 d-lg-none"></i>
                    <span class="nav-link-inner--text">产品列表</span>
                </a>

                <a slot="title" href="/#/About" class="nav-link" role="button">
                    <i class="ni ni-ui-04 d-lg-none"></i>
                    <span class="nav-link-inner--text">关于我们</span>
                </a>
            </ul>
            <ul class="navbar-nav align-items-lg-center ml-lg-auto">

                <li class="nav-item d-none d-lg-block ml-lg-4">
                    <a href="https://www.creative-tim.com/product/vue-argon-design-system" target="_blank"
                        rel="noopener" class="btn btn-neutral btn-icon">
                        <span class="btn-inner--icon">
                            <i class="fa fa-cloud-download mr-2"></i>
                        </span>
                        <span class="nav-link-inner--text">联系我们</span>
                    </a>
                </li>
            </ul>
        </base-nav>
    </header>
</template>
<script>
import BaseNav from "@/components/BaseNav";
import BaseDropdown from "@/components/BaseDropdown";
import CloseButton from "@/components/CloseButton";

export default {
    components: {
        BaseNav,
        CloseButton,
        BaseDropdown
    }
};
</script>
<style></style>
