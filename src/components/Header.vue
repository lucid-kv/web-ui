<template>
<div id="header" class="page-header ">
    <div class="navbar navbar-expand-lg">
        <!-- brand -->
        <a href="index.html" class="navbar-brand d-lg-none">
            <svg width="32" height="32" viewBox="0 0 512 512" xmlns="http://www.w3.org/2000/svg" fill="currentColor">
                <g class="loading-spin" style="transform-origin: 256px 256px">
                    <path
                        d="M200.043 106.067c-40.631 15.171-73.434 46.382-90.717 85.933H256l-55.957-85.933zM412.797 288A160.723 160.723 0 0 0 416 256c0-36.624-12.314-70.367-33.016-97.334L311 288h101.797zM359.973 134.395C332.007 110.461 295.694 96 256 96c-7.966 0-15.794.591-23.448 1.715L310.852 224l49.121-89.605zM99.204 224A160.65 160.65 0 0 0 96 256c0 36.639 12.324 70.394 33.041 97.366L201 224H99.204zM311.959 405.932c40.631-15.171 73.433-46.382 90.715-85.932H256l55.959 85.932zM152.046 377.621C180.009 401.545 216.314 416 256 416c7.969 0 15.799-.592 23.456-1.716L201.164 288l-49.118 89.621z">
                    </path>
                </g>
            </svg>
            <!-- <img src="<%= BASE_URL %>img/logo.png" alt="..."> -->
            <span class="hidden-folded d-inline l-s-n-1x d-lg-none">Basik</span>
        </a>
        <div class="collapse navbar-collapse order-2 order-lg-1" id="navbarToggler">
            <form class="input-group m-2 my-lg-0 ">
                <div class="input-group-prepend">
                    <button type="button" class="btn no-shadow no-bg px-0 text-inherit">
                        <i data-feather="search"></i>
                    </button>
                </div>
                <input type="text" class="form-control no-border no-shadow no-bg typeahead" placeholder="Search components..." data-plugin="typeahead" data-api="<%= BASE_URL %>api/menu.json">
            </form>
        </div>
        <ul class="nav navbar-menu order-1 order-lg-2">
            <li class="nav-item d-none d-sm-block">
                <a class="nav-link px-2" data-toggle="fullscreen" data-plugin="fullscreen">
                    <i data-feather="maximize"></i>
                </a>
            </li>
            <li class="nav-item dropdown">
                <a class="nav-link px-2" data-toggle="dropdown">
                    <i data-feather="settings"></i>
                </a>
                <!-- ############ Setting START-->
                <div class="dropdown-menu dropdown-menu-center mt-3 w-md animate fadeIn">
                    <div class="setting px-3">
                        <div class="mb-2 text-muted">
                            <strong>Setting:</strong>
                        </div>
                        <div class="mb-3" id="settingLayout">
                            <label class="ui-check ui-check-rounded my-1 d-block">
                                <input type="checkbox" name="stickyHeader">
                                <i></i>
                                <small>Sticky header</small>
                            </label>
                            <label class="ui-check ui-check-rounded my-1 d-block">
                                <input type="checkbox" name="stickyAside">
                                <i></i>
                                <small>Sticky aside</small>
                            </label>
                            <label class="ui-check ui-check-rounded my-1 d-block">
                                <input type="checkbox" name="foldedAside">
                                <i></i>
                                <small>Folded Aside</small>
                            </label>
                            <label class="ui-check ui-check-rounded my-1 d-block">
                                <input type="checkbox" name="hideAside">
                                <i></i>
                                <small>Hide Aside</small>
                            </label>
                        </div>
                        <div class="mb-2 text-muted">
                            <strong>Color:</strong>
                        </div>
                        <div class="mb-2">
                            <label class="radio radio-inline ui-check ui-check-md">
                                <input type="radio" name="bg" value="">
                                <i></i>
                            </label>
                            <label class="radio radio-inline ui-check ui-check-color ui-check-md">
                                <input type="radio" name="bg" value="bg-dark">
                                <i class="bg-dark"></i>
                            </label>
                        </div>
                        <div class="mb-2 text-muted">
                            <strong>Layouts:</strong>
                        </div>
                        <div class="mb-3">
                            <a href="dashboard.html" class="btn btn-xs btn-white no-ajax mb-1">Default</a>
                            <a href="layout.a.html?bg" class="btn btn-xs btn-primary no-ajax mb-1">A</a>
                            <a href="layout.b.html?bg" class="btn btn-xs btn-info no-ajax mb-1">B</a>
                            <a href="layout.c.html?bg" class="btn btn-xs btn-success no-ajax mb-1">C</a>
                            <a href="layout.d.html?bg" class="btn btn-xs btn-warning no-ajax mb-1">D</a>
                        </div>
                        <div class="mb-2 text-muted">
                            <strong>Apps:</strong>
                        </div>
                        <div>
                            <a href="dashboard.html" class="btn btn-sm btn-white no-ajax mb-1">Dashboard</a>
                            <a href="music.html?bg" class="btn btn-sm btn-white no-ajax mb-1">Music</a>
                            <a href="video.html?bg" class="btn btn-sm btn-white no-ajax mb-1">Video</a>
                        </div>
                    </div>
                </div>
                <!-- ############ Setting END-->
            </li>
            <!-- Notification -->
            <li class="nav-item dropdown">
                <a class="nav-link px-2 mr-lg-2" data-toggle="dropdown">
                    <i data-feather="bell"></i>
                    <span class="badge badge-pill badge-up bg-primary">5</span>
                </a>
                <!-- dropdown -->
                <div class="dropdown-menu dropdown-menu-right mt-3 w-md animate fadeIn p-0">
                    <div class="scrollable hover" style="max-height: 250px">
                        <div class="list list-row">
                            <div class="list-item " data-id="11">
                                <div>
                                    <a href="#">
                                        <span class="w-32 avatar gd-info">
                                            K
                                        </span>
                                    </a>
                                </div>
                                <div class="flex">
                                    <div class="item-feed h-2x">
                                        Prepare the documentation for the
                                        <a href='#'>Fitness app</a>
                                    </div>
                                </div>
                            </div>
                            <div class="list-item " data-id="14">
                                <div>
                                    <a href="#">
                                        <span class="w-32 avatar gd-warning">
                                            B
                                        </span>
                                    </a>
                                </div>
                                <div class="flex">
                                    <div class="item-feed h-2x">
                                        Do you know which are the popular ones? Leave a comment and get to know more from professional developers
                                    </div>
                                </div>
                            </div>
                            <div class="list-item " data-id="17">
                                <div>
                                    <a href="#">
                                        <span class="w-32 avatar gd-warning">
                                            H
                                        </span>
                                    </a>
                                </div>
                                <div class="flex">
                                    <div class="item-feed h-2x">
                                        AI will deliver adaptive learning processes in assessments & digital textbooks to personalize learning
                                    </div>
                                </div>
                            </div>
                            <div class="list-item " data-id="10">
                                <div>
                                    <a href="#">
                                        <span class="w-32 avatar gd-danger">
                                            <img src="<%= BASE_URL %>img/a10.jpg" alt=".">
                                        </span>
                                    </a>
                                </div>
                                <div class="flex">
                                    <div class="item-feed h-2x">
                                        Developers of
                                        <a href='#'>@iAI</a>, the AI assistant based on Free Software
                                    </div>
                                </div>
                            </div>
                            <div class="list-item " data-id="20">
                                <div>
                                    <a href="#">
                                        <span class="w-32 avatar gd-warning">
                                            G
                                        </span>
                                    </a>
                                </div>
                                <div class="flex">
                                    <div class="item-feed h-2x">
                                        <a href='#'>@Netflix</a> hackathon
                                    </div>
                                </div>
                            </div>
                            <div class="list-item " data-id="17">
                                <div>
                                    <a href="#">
                                        <span class="w-32 avatar gd-warning">
                                            A
                                        </span>
                                    </a>
                                </div>
                                <div class="flex">
                                    <div class="item-feed h-2x">
                                        Alibaba made a smart screen
                                        <a href='#'>@Alibaba</a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="d-flex px-3 py-2 b-t">
                        <div class="flex">
                            <span>6 Notifications</span>
                        </div>
                        <a href="page.setting.html">See all
                            <i class="fa fa-angle-right text-muted"></i>
                        </a>
                    </div>
                </div>
                <!-- / dropdown -->
            </li>
            <!-- User dropdown menu -->
            <li class="nav-item dropdown">
                <a href="#" data-toggle="dropdown" class="nav-link d-flex align-items-center px-2 text-color">
                    <span class="avatar w-24" style="margin: -2px;"><img src="/img/a1.jpg" alt="..."></span>
                </a>
                <div class="dropdown-menu dropdown-menu-right w mt-3 animate fadeIn">
                    <a class="dropdown-item" href="page.profile.html">
                        <span>Jacqueline Reid</span>
                    </a>
                    <a class="dropdown-item" href="page.price.html">
                        <span class="badge bg-success text-uppercase">Upgrade</span>
                        <span>to Pro</span>
                    </a>
                    <div class="dropdown-divider"></div>
                    <a class="dropdown-item" href="page.profile.html">
                        <span>Profile</span>
                    </a>
                    <a class="dropdown-item d-flex" href="page.invoice.html">
                        <span class="flex">Invoice</span>
                        <span><b class="badge badge-pill gd-warning">5</b></span>
                    </a>
                    <a class="dropdown-item" href="page.faq.html">Need help?</a>
                    <div class="dropdown-divider"></div>
                    <a class="dropdown-item" href="page.setting.html">
                        <span>Account Settings</span>
                    </a>
                    <a class="dropdown-item" href="signin.html">Sign out</a>
                </div>
            </li>
            <li class="nav-item d-lg-none">
                <a href="#" class="nav-link px-2" data-toggle="collapse" data-toggle-class data-target="#navbarToggler">
                    <i data-feather="search"></i>
                </a>
            </li>
            <li class="nav-item d-lg-none">
                <a class="nav-link px-1" data-toggle="modal" data-target="#aside">
                    <i data-feather="menu"></i>
                </a>
            </li>
        </ul>
    </div>
</div>
</template>

<script>
export default {
  name: 'Header',
  props: {
  }
}
</script>
