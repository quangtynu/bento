# Bento Releases
## Version 15.7.0
_2020-02-05_
* New: Add a registerItemVisibilityListener to Component, to avoid needing to override components simply for that. (Comes bundled with an unregister method)
* Fix: Change CarouselComponent behavior so that it notifies it's nested Components when it becomes visible or invisible because of scrolling.

## Version 15.6.0
_2020-01-27_
* Fix: Change NestedComponent to have separate presenter from its inner Component.

## Version 15.5.0
_2020-01-16_
* New: Add remove() and clear() functions to CarouselComponent.
* New: Add a unit test for testing CarouselComponent's add(), addAll(), remove(), and clear() functions.

## Version 15.4.0
_2019-12-18_
* New: Add a NestedComponent that can be used for nesting a given inner Component inside a given outer ViewHolder.

## Version 15.3.2
_2019-10-08_
* Fix: Fixed bug in ListItemTouchCallback causing crash when viewHolder.adapterPosition is -1
* Fix: Add detailed exception thrown when AccordionList.rangedValueAt is called with an incorrect value.

## Version 15.3.1
_2019-08-29_
* Fix: Fixed appending data to ListComponent.
* Fix: Fixed issue where we were no longer sharing the RecyclePool in CarouselComponent.
* Fix: Fixed unit and espresso tests. No more PowerMock.

## Version 15.3.0
_2019-08-13_
* Behavior change: CarouselComponent now remembers its scroll position when it's scrolled offscreen.

## Version 15.2.0
_2019-08-07_
* New: Added TabViewPagerComponent to use both TabLayout and ViewPager in one view.

## Version 15.1.1
_2019-07-11_
* Fix: Add check for gap in ComponentGroup ([#20](https://github.com/Yelp/bento/pull/20))

## Version 15.1.0
_2019-07-11_
* New: Add support for drag and drop for RecyclerViews.

## Version 15.0.0
_2019-05-20_
* Behavior change: ListComponent callback for onItemVisible will only be called on items, not on separators.

## Version 14.1.0 
_2019-05-03_

* Behavior change: when inserting a component or item at index 0, the RecyclerViewComponentController will keep the RecyclerView scrolled on top if it was currently showing the item at index 0.

## Version 14.0.0
_2019-04-18_

* First official Bento public release.
