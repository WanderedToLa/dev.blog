# Front에서 modal관리하기

1. slice(Redux)하나로 관리
2. React-portal
3. html popover

## Popover

얼마전에 생긴 `popover`를 알게되었는데 이걸로 모달을 관리하면 좋아보인다.  
5월에 실험단계였는데 현재는 출시된 상태.

기본적으로 `display:none`속성  
`<button>` 이나 `<input type='button'>` 을통해 호출하거나 `HTMLElement.showPopover()`를 통해서 호출가능하다.  
호출이 되었을때 다른 모든 요소위에 표시되면서 상위스타일에 영향받지 않는다.

```html
<button popovertarget="my-popover">Open Popover</button>

<div popover id="my-popover">My Popover</div>
```

- [Semantics and the popover attribute: what to use when?](https://hidde.blog/popover-semantics/)
