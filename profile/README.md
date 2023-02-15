## Hi there 👋

While looking at [modularizing](https://github.com/rust-mobile/ndk/issues/372) the [`android-ndk-rs`](https://github.com/rust-mobile/ndk) repo (that used to be hosted under the [rust-windowing](https://github.com/rust-windowing) org), we decided to create this `rust-mobile` organisation as a place to foster collaboration and coordinate work on crates that are aimed at supporting mobile application development with Rust (i.e. Android and iOS)

The general motivation for this was:

1. To help make smaller utility crates a little easier to discover
2. More easily share ideas / patterns between crates where it makes sense. E.g. use the organisaiton discussion boards to solicit feedback from developers working on related crates.
3. Help share the maintenance burden if wanted (E.g. in case someone no longer has the time / bandwidth / interest to work on a crate)

Thinking about Android specifically we can see that there are some cross-cutting issues that we haven't got good answers for yet, including:
1. no standard way of communicating whether libstdc++ is linked statically or shared
2. no standard way of dealing with SDK versioning so crates know what Android APIs they should target
3. no good (consistent + ergonomic) way yet for passing around `JavaVM` and `Activity` pointers for making JNI calls

The hope is that this organisation can help foster collaboration, so we can address these kinds of things consistently.

# Join us, we have cookies 🍪

If you have a Rust crate that's primarily aimed at mobile app development we invite you to open an issue [here](https://github.com/rust-mobile/.github/issues) to discus re-homing here.

Alternatively open an issue against your own repo to discuss and poke me (@rib) or any of the other org owners here: https://github.com/orgs/rust-mobile/people

For anyone interested in moving a repo here; you'd still have responsibility over your own project as the maintainer. There's no obligation to give other members joint maintainer priviledges over your project (though it's hopefully a good opportunity to find collaborators).
