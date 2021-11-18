<template>
    {{-- this component for the header --}}
    <div id="app">
        <nav class="navbar navbar-expand navbar-light fixed-top">
            <div class="container">
                <a href="#" class="navbar-brand">home</a>
                <div class="collapse navbar-collapse">
                    <ul class="navbar-nav ml-auto">
                        <li class="nav-item">
                            <a href="#" class="nav-link">login</a>
                        </li>
                        <li class="nav-item">
                            <a href="#" class="nav-link">sign up</a>
                            <modal name="modal-login">
                                hello, world
                            </modal>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </div>
</template>
<script>
    export default {
        name: 'Nav'
    }

</script>
