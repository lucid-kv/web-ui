<template>
    <div id="aside" class="page-sidenav no-shrink bg-light nav-dropdown fade" aria-hidden="true">
        <div class="sidenav h-100 modal-dialog bg-light">
            <div class="navbar">
                <a href="/" class="navbar-brand ">
                    <img src="/img/logo.png" style="width: 24px; padding-bottom: 2px;" alt="Lucid KV">
                    <span class="hidden-folded d-inline l-s-n-1x ">Lucid KV</span>
                </a>
            </div>
            <div class="flex scrollable hover">
                <div class="nav-active-text-primary" data-nav>
                    <ul class="nav bg">
                        <li class="nav-header hidden-folded">
                            <span class="text-muted">Main</span>
                        </li>
                        <li>
                            <a href="dashboard.html">
                                <span class="nav-icon text-primary"><i data-feather='home'></i></span>
                                <span class="nav-text">Dashboard</span>
                            </a>
                        </li>
                        <li class="nav-header hidden-folded">
                            <span class="text-muted">Instance</span>
                        </li>
                        <li>
                            <a href="app.calendar.html">
                                <span class="nav-icon text-info"><i data-feather='database'></i></span>
                                <span class="nav-text">KV Store</span>
                                <!-- <span class="nav-badge"><b class="badge-circle xs text-danger"></b></span> -->
                            </a>
                        </li>
                        <li>
                            <a href="app.user.html">
                                <span class="nav-icon text-success"><i data-feather='users'></i></span>
                                <span class="nav-text">Authentication</span>
                            </a>
                        </li>
                        <li>
                            <a href="app.message.html">
                                <span class="nav-icon text-warning"><i data-feather='bell'></i></span>
                                <span class="nav-text">Notifications</span>
                                <!-- <span class="nav-badge"><b class="badge-circle xs text-warning"></b></span> -->
                            </a>
                        </li>
                        <li>
                            <a href="app.mail.html">
                                <span class="nav-icon text-danger"><i data-feather='settings'></i></span>
                                <span class="nav-text">Node Settings</span>
                            </a>
                        </li>
                    </ul>
                    <ul class="nav ">
                        <li class="nav-header hidden-folded">
                            <span class="text-muted">Features</span>
                        </li>
                        <li>
                            <a href="#" class="text-muted">
                                <span class="nav-icon"><i data-feather='archive'></i></span>
                                <span class="nav-text">Persistence</span>
                            </a>
                        </li>
                        <li>
                            <a href="#" class="text-muted">
                                <span class="nav-icon"><i data-feather='activity'></i></span>
                                <span class="nav-text">Monitoring</span>
                            </a>
                        </li>
                        <li>
                            <a href="#" class="text-muted">
                                <span class="nav-icon"><i data-feather='terminal'></i></span>
                                <span class="nav-text">Command Line</span>
                            </a>
                        </li>
                        <li>
                            <a href="#" class="text-muted">
                                <span class="nav-icon"><i data-feather='zap'></i></span>
                                <span class="nav-text">Encryption</span>
                            </a>
                        </li>
                        <li>
                            <a href="#" class="text-muted">
                                <span class="nav-icon"><i data-feather='sunset'></i></span>
                                <span class="nav-text">Compression</span>
                            </a>
                        </li>
                    </ul>
                    <ul class="nav ">
                        <li class="nav-header hidden-folded">
                            <span class="text-muted">Community</span>
                        </li>
                        <li>
                            <a href="#" class="">
                                <span class="nav-icon"><i data-feather='github'></i></span>
                                <span class="nav-text">GitHub Repository</span>
                            </a>
                        </li>
                        <li>
                            <a href="#" class="">
                                <span class="nav-icon"><i data-feather='book-open'></i></span>
                                <span class="nav-text">Documentation</span>
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="no-shrink ">
                <div class="p-3 d-flex align-items-center">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'NavMenu',
  props: {
  }
}
</script>
