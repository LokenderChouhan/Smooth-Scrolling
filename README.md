# Smooth Scrolling Page

Here “smooth scrolling” we don’t mean smoothly scrolling to an element, but rather a smoothly animated kind of scrolling behavior. With addition of “inner” image animation that adds another interesting layer to the whole scroll movement.

## Why?
If you have ever animated something on scroll, you might have experienced that browsers have difficulties in displaying the incoming content jank-free; especially images may show tiny abrupt jumps on scroll. It just feel easy on the eye. 

To avoid that, we can use the trick of animating the content itself by translating it up or down instead of using the “native” scroll.

## Implementaion.

1.  A content wrapper is set to position fixed with the overflow set to hidden so that its child ( here image div ) can be moved.
2. When we scroll, the fixed wrapper will stay in place while we animate the inner content.
3. The body will get the height of the content set to it, so that we preserve the scroll bar.

## Outcome

This trick makes a simple yet effective smooth scrolling behavior possible.

It’s not inherently changing scroll behavior, but simply subtly modifying the experience to make it smoother and more enjoyable.

## Issues.

 Scroll jacking (one that prevents fast swiping up or down a page on mobile) 

 This effect is not suited for mobile. Just as with every other design choice, it depends on the context.

 But simply stating “scrolljacking is bad”, is too simplistic for todays standards.
 
## Preview

https://lokenderchouhan.github.io/

