Example project with a rust webserver (warp) serving a rust frontend (yew) as wasm included in the webserver binary using include_bytes.

This is motivated by a desire to share code and types between the frontend (wasm) and native backend code, so it's all in a single workspace.

currently requires latest rust nightly or higher (due to bug fix for a stable regression, not for experimental features)

TODO:
- revise web server section - mildly janky, more of a proof of concept
- FIXED: use phf instead of lazy_static after https://github.com/rust-lang/rust/issues/70584 is resolved 
- mark as non-nightly only when the fix to that issue hits stable
