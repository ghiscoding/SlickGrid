Clone the repo
```bash
git clone https://github.com/ghiscoding/SlickGrid
```

Then open the demo from the folder `slickgrid/examples/example-tree-data.html` and run it 

TODO
1. Seems that `filterMyFiles()` returns duplicate results, so for now I call `uniqueArray()` to remove any duplicates
   - would be nice to avoid having to dedupe but I can also live with it, not a huge problem
2. I manage to get the demo working, the `myFilter()` calls the `var tmpResult = filterMyFiles()` and then I do a `tmpResult.find()` to see if the object Id is in the array, I return true/false with that in mind
   - perhaps `filterMyFiles()` could simply store the object Ids? That might improve search quite a lot
3. The code requires `eval` of `Function('return '...')` which is unsafe, can that be replaced?
4. I copied Alex's code before this message, so I'm not sure what changed.
> Done! Haha brain was still thinking about the problem. Just need to delete each key, value from myObj once it’s used. No further iteration needed :) – Alex L

I opened an issue [#1](https://github.com/ghiscoding/SlickGrid/issues/1) for tracking, we can discuss there if you wish.

THANKS A LOT!!!