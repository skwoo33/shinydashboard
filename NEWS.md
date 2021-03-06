shinydashboard 0.5.3.9000
=========================

* Fixed [#89](https://github.com/rstudio/shinydashboard/issues/89): We claimed that `dashboardPage()` would try to extract the page's title from `dashboardHeader()` (if the title is not provided directly to `dashboardPage()`); however, we were selecting the wrong child of the header tag object ([#203](https://github.com/rstudio/shinydashboard/pull/203))
	
* Fixed [#129](https://github.com/rstudio/shinydashboard/issues/129): Trigger shown/hidden event for Shiny outputs in the sidebar. ([#194](https://github.com/rstudio/shinydashboard/pull/194))
	
* Fixed [#73](https://github.com/rstudio/shinydashboard/issues/73): add `collapsed` argument to `dashboardSidebar()`, which allows it to start off collapsed. ([#186](https://github.com/rstudio/shinydashboard/pull/186))

* Fixed [#62](https://github.com/rstudio/shinydashboard/issues/62): make images resize when the sidebar collapses/expands. [#185](https://github.com/rstudio/shinydashboard/pull/185)

* Addressed [#178](https://github.com/rstudio/shinydashboard/issues/178): switch from `npm` to `yarn`. Also upgraded all yarn packages to the `latest` tag (all major changes). [#184](https://github.com/rstudio/shinydashboard/pull/184)

* Fixed [#176](https://github.com/rstudio/shinydashboard/issues/176) (making buttons look good on the sidebar) by giving Shiny action buttons and links some margin space. ([#182](https://github.com/rstudio/shinydashboard/pull/182))

* Updated to AdminLTE 2.3.11. ([#181](https://github.com/rstudio/shinydashboard/pull/181))

shinydashboard 0.5.3
=========================

* Fixed ([#160](https://github.com/rstudio/shinydashboard/issues/160): Using a dynamically-created `sidebarMenu` without an `id` argument would cause the app to not start, when used with Shiny 0.14.

shinydashboard 0.5.2
====================

* Added ability to bookmark and restore tabs, when used with Shiny 0.14 and above. ([#152](https://github.com/rstudio/shinydashboard/issues/152), [#157](https://github.com/rstudio/shinydashboard/pull/157))

* Fixed issue with R CMD check and Shiny version 0.14.

* Updated to AdminLTE 2.3.2 (1ee281b).

shinydashboard 0.5.1
====================

* Logout panels from Shiny Server Pro were previously not visible, but now they are.

* If a `sidebarUserPanel` doesn't have an image, space for the image is no longer allocated.

* `tabNames` are now validated so that illegal characters result in an error early. (#66)

* `sidebarUserPanel` now displays properly. (#70)

* `radioButtons` did not wrap, but now they do. (#60)

shinydashboard 0.5.0
====================

* Updated to AdminLTE 2.1.2 (406de4e). Please note that some CSS selectors have changed, so if you are using custom CSS, it may require modification. The documentation at http://rstudio.github.io/shinydashboard/appearance.html has some updated examples.

* shinydashboard now respects the `shiny.minified` option.

* Collapse buttons on boxes trigger `shown` and `hidden` events. Previously they did not, which resulted in dynamic content not working for boxes that started collapsed. (#17, #42)

* Dynamic menuSubItems now work in the sidebar. (#54)

* Arbitrary content may now be used in a `sidebarMenu()`, not just `menuItem`s. (#44)

* Added options to set the width of `dashboardHeader()` and `dashboardSidebar()`. (#43, #45, #54)
