# Comparing `tmp/fixed2float-3.0.0_rc1.tar.gz` & `tmp/fixed2float-4.0.0_rc1.tar.gz`

## Comparing `fixed2float-3.0.0_rc1.tar` & `fixed2float-4.0.0_rc1.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 fixed2float-3.0.0_rc1/local_dependencies/fixed2float/Cargo.toml
--rw-r--r--   0     1001      121     1269 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/local_dependencies/fixed2float/README.md
--rw-r--r--   0     1001      121      891 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/local_dependencies/fixed2float/examples/basic.rs
--rw-r--r--   0     1001      121     3131 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/local_dependencies/fixed2float/src/fixed_point/fx_fx.rs
--rw-r--r--   0     1001      121     3777 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/local_dependencies/fixed2float/src/fixed_point/fx_q.rs
--rw-r--r--   0     1001      121     3566 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/local_dependencies/fixed2float/src/fixed_point.rs
--rw-r--r--   0     1001      121     8109 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/local_dependencies/fixed2float/src/lib.rs
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 fixed2float-3.0.0_rc1/Cargo.toml
--rw-r--r--   0     1001      121      224 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/.cargo/config
--rw-r--r--   0     1001      121      779 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/Makefile
--rw-r--r--   0        0        0     1269 2022-04-09 08:56:32.000000 fixed2float-3.0.0_rc1/README.md
--rw-r--r--   0     1001      121      553 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/examples/example.py
--rw-r--r--   0     1001      121     8407 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/examples/notebook.ipynb
--rw-r--r--   0     1001      121      424 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/fixed2float/__init__.py
--rw-r--r--   0     1001      121      571 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/pyproject.toml
--rw-r--r--   0     1001      121     2923 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/src/lib.rs
--rw-r--r--   0     1001      121      103 2022-04-09 08:56:31.000000 fixed2float-3.0.0_rc1/tests.py
--rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 fixed2float-3.0.0_rc1/PKG-INFO
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 fixed2float-4.0.0_rc1/local_dependencies/fixed2float/Cargo.toml
+-rw-r--r--   0     1001      123       14 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/local_dependencies/fixed2float/.rustfmt.toml
+-rw-r--r--   0     1001      123     1205 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/local_dependencies/fixed2float/README.md
+-rw-r--r--   0     1001      123     1214 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/local_dependencies/fixed2float/examples/basic.rs
+-rw-r--r--   0     1001      123      301 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/local_dependencies/fixed2float/examples/operations.rs
+-rw-r--r--   0     1001      123     3944 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/local_dependencies/fixed2float/src/fixed_point/fx_fx.rs
+-rw-r--r--   0     1001      123     3470 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/local_dependencies/fixed2float/src/fixed_point/fx_q.rs
+-rw-r--r--   0     1001      123     3519 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/local_dependencies/fixed2float/src/fixed_point.rs
+-rw-r--r--   0     1001      123     8945 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/local_dependencies/fixed2float/src/lib.rs
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 fixed2float-4.0.0_rc1/Cargo.toml
+-rw-r--r--   0     1001      123      224 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/.cargo/config
+-rw-r--r--   0     1001      123       97 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/CHANGELOG.md
+-rw-r--r--   0     1001      123      772 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/Makefile
+-rw-r--r--   0        0        0     1205 2023-05-08 12:02:04.000000 fixed2float-4.0.0_rc1/README.md
+-rw-r--r--   0     1001      123      553 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/examples/example.py
+-rw-r--r--   0     1001      123    11435 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/examples/notebook.ipynb
+-rw-r--r--   0     1001      123     1057 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/fixed2float/__init__.py
+-rw-r--r--   0     1001      123      608 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/pyproject.toml
+-rw-r--r--   0     1001      123     2996 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/src/lib.rs
+-rw-r--r--   0     1001      123      103 2023-05-08 12:02:03.000000 fixed2float-4.0.0_rc1/tests.py
+-rw-r--r--   0        0        0     1629 1970-01-01 00:00:00.000000 fixed2float-4.0.0_rc1/PKG-INFO
```

### Comparing `fixed2float-3.0.0_rc1/local_dependencies/fixed2float/Cargo.toml` & `fixed2float-4.0.0_rc1/local_dependencies/fixed2float/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "fixed2float"
-version = "3.0.0-rc1"
+version = "4.0.0-rc1"
 authors = ["Francesco Urbani <francescourbanidue@gmail.com>"]
 edition = "2021"
 keywords = ["fixed", "float", "q-format"]
 documentation = "https://docs.rs/fixed2float"
 # homepage = ""
 license = "MIT"
 readme = "README.md"
```

### Comparing `fixed2float-3.0.0_rc1/local_dependencies/fixed2float/README.md` & `fixed2float-4.0.0_rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,45 @@
+Metadata-Version: 2.1
+Name: fixed2float
+Version: 4.0.0_rc1
+Summary: Fixed point to floating point conversion utility
+Keywords: fixed,float,q-format
+Author: Francesco Urbani <francescourbanidue@gmail.com>
+Author-email: Francesco Urbani <francescourbanidue@gmail.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/urbanij/fixed2float
+
+# fixed2float
 [![Crates.io](https://img.shields.io/crates/v/fixed2float)](https://crates.io/crates/fixed2float)
 [![PyPI](https://img.shields.io/pypi/v/fixed2float)](https://pypi.org/project/fixed2float/)
+[![codecov](https://codecov.io/gh/urbanij/fixed2float/branch/master/graph/badge.svg?token=9JEMJTB2IT)](https://codecov.io/gh/urbanij/fixed2float)
 
-# fixed2float
 
-Simple utility for fixed point to real number conversions, using the VisSim (Fx*m.b*) and Q (Q*m.n*) [notations](https://en.wikipedia.org/wiki/Fixed-point_arithmetic#Notations).
+Simple utility for fixed point to real number conversions, using the VisSim (Fx*m.b*) ~~and Q (Q*m.n*)~~ [notation](https://en.wikipedia.org/wiki/Fixed-point_arithmetic#Notations).
 
 ### Usage
 
 - as a dependency of your Rust library
 
 ```sh
 cargo add fixed2float
 ```
 
-which will automatically fetch the most recent version from the registry and update one line on Cargo.toml.
-
 - as a dependency of your Python library
 
 ```sh
 pip install fixed2float
 ```
 
 
 ### Examples
+- Interactive notebook [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/urbanij/fixed2float/HEAD?labpath=py-fixed2float%2Fexamples%2Fnotebook.ipynb)
+- [example.py](https://github.com/urbanij/fixed2float/blob/master/py-fixed2float/examples/example.py) (Python)
+- [examples folder](https://github.com/urbanij/fixed2float/tree/master/examples) (Rust) 
 
-See [example.py](https://github.com/urbanij/fixed2float/blob/master/py-fixed2float/examples/example.py) (Python) or the [examples folder](https://github.com/urbanij/fixed2float/tree/master/examples) (Rust) or this online notebook:
-
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/urbanij/fixed2float/HEAD?labpath=py-fixed2float%2Fexamples%2Fnotebook.ipynb)
 
 <!-- ### Screencast -->
 
 <!-- [![asciicast](https://asciinema.org/a/463661.svg)](https://asciinema.org/a/463661) -->
 
 
-### Similar projects
-
-- [javascript's fixed2float](https://www.npmjs.com/package/fixed2float)
```

### Comparing `fixed2float-3.0.0_rc1/local_dependencies/fixed2float/src/fixed_point/fx_fx.rs` & `fixed2float-4.0.0_rc1/local_dependencies/fixed2float/src/fixed_point/fx_q.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,130 +1,142 @@
 use super::FixedPoint;
 use crate::{fixed_point::debug_print, mask, to_float, UInt};
 
+//#[deprecated(since="4.0.0", note="Use `Fx` instead")]
 #[derive(PartialEq, Eq, Clone, Copy)]
-pub struct Fx {
-    pub val: UInt,
-    pub m: i32,
-    pub b: i32,
-    pub is_exact: bool,
-}
-
-impl Fx {
-    pub fn new(val: UInt, m: i32, b: i32, is_exact: bool) -> Self {
-        if b < m {
-            panic!("Total num of bits must be larger than num of integer bits.")
-        }
-        Self {
-            val,
-            m,
-            b,
-            is_exact,
-        }
-    }
-
-    pub fn get_frac_bits(&self) -> i32 {
-        self.b - self.m
-    }
-}
-
-impl FixedPoint for Fx {
-    fn eval(&self) -> f64 {
-        to_float(self.val, self.b, self.m, self.b - self.m).unwrap()
-    }
-}
-
-impl std::ops::Shl<u32> for Fx {
-    type Output = Self;
-    fn shl(self, rhs: u32) -> Self::Output {
-        Self {
-            val: (self.val << rhs) & mask((self.b) as u32) as UInt,
-            m: self.m,
-            b: self.b,
-            is_exact: self.is_exact,
-        }
-    }
-}
-
-impl std::ops::Shr<u32> for Fx {
-    type Output = Self;
-    fn shr(self, rhs: u32) -> Self::Output {
-        // let val = (self.val >> rhs) & mask((self.b) as u32) as u64;
-        let val = match self.val.checked_shr(rhs) {
-            Some(v) => v & mask((self.b) as u32) as UInt,
-            None => 0,
-        };
-
-        Self {
-            val,
-            m: self.m,
-            b: self.b,
-            is_exact: self.is_exact,
-        }
-    }
-}
-
-impl std::ops::Add for Fx {
-    type Output = Self;
-    fn add(self, rhs: Self) -> Self::Output {
-        if self.m != rhs.m || self.b != rhs.b {
-            panic!("`m` and `n` field of each fx obj has to match.")
-        }
-        Self {
-            val: self.val + rhs.val,
-            m: self.m + 1,
-            b: self.b + 1,
-            is_exact: true,
-        }
-    }
-}
-
-impl std::ops::Sub for Fx {
-    type Output = Self;
-    fn sub(self, rhs: Self) -> Self::Output {
-        if rhs.eval() > self.eval() {
-            unimplemented!()
-        }
-        Self {
-            val: self.val - rhs.val,
-            m: self.m,
-            b: self.b,
-            is_exact: true,
-        }
-    }
-}
-
-impl std::ops::Mul for Fx {
-    type Output = Self;
-    fn mul(self, rhs: Self) -> Self::Output {
-        Self {
-            val: self.val * rhs.val,
-            m: self.m + rhs.m,
-            b: self.b + rhs.b,
-            is_exact: true,
-        }
-    }
-}
-
-impl std::fmt::Debug for Fx {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        let ans = debug_print(self.val, self.m, self.b, self.is_exact);
-        write!(f, "{}", ans)
-    }
-}
-
-impl std::fmt::Display for Fx {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        let ans;
-        ans = format!("Fx<{},{}>({})", self.m, self.b, self.val);
-        write!(f, "{}", ans)
-    }
+pub struct Q {
+  pub val: UInt,
+  pub m: i32,
+  pub n: i32,
+  pub is_exact: bool,
+}
+
+impl Q {
+  pub fn new(val: UInt, m: i32, n: i32, is_exact: bool) -> Self {
+    Self {
+      val,
+      m,
+      n,
+      is_exact,
+    }
+  }
+}
+
+impl FixedPoint for Q {
+  fn eval(&self) -> f64 {
+    to_float(self.val, self.m + self.n, self.m, self.n).unwrap()
+  }
+
+  // fn index(&self, _range: std::ops::Range<usize>) -> Result<Self, String> {
+  //         use super::mask;
+
+  //         let (left_idx, right_idx) = (range.start + 1, range.end);
+  //         if left_idx < right_idx {
+  //             return Err("Left index can't be larger than right index".to_string());
+  //         }
+  //         let range_size = (left_idx - right_idx) as i32;
+
+  //         if left_idx as i32 > self.m + self.n {
+  //             return Err("Left index can't be larger than fixed point number itself".to_string());
+  //         }
+  //         if range_size == 0 {
+  //             return Err("Range can't be null".to_string());
+  //         }
+
+  //         let new_val = (self.val >> right_idx) & mask(left_idx as u128);
+  //         let new_n = std::cmp::max(0, self.n - right_idx as i32 );
+  //         let new_m = range_size - new_n;
+  //         Ok(Self {
+  //             val: new_val,
+  //             m: new_m,
+  //             n: new_n,
+  //             is_exact: true,
+  //         })
+  //     unimplemented!()
+  // }
+}
+
+impl std::ops::Shl<u32> for Q {
+  type Output = Self;
+  fn shl(self, rhs: u32) -> Self::Output {
+    Self {
+      val: (self.val << rhs) & mask((self.m + self.n) as u32) as UInt,
+      m: self.m,
+      n: self.n,
+      is_exact: self.is_exact,
+    }
+  }
+}
+
+impl std::ops::Shr<u32> for Q {
+  type Output = Self;
+  fn shr(self, rhs: u32) -> Self::Output {
+    Self {
+      val: (self.val >> rhs) & mask((self.m + self.n) as u32) as UInt,
+      m: self.m,
+      n: self.n,
+      is_exact: self.is_exact,
+    }
+  }
+}
+
+impl std::ops::Add for Q {
+  type Output = Self;
+  fn add(self, rhs: Self) -> Self::Output {
+    if self.m != rhs.m || self.n != rhs.n {
+      panic!("`m` and `n` field of each Fx obj must match.")
+    }
+    Self {
+      val: self.val + rhs.val,
+      m: self.m + 1,
+      n: self.n,
+      is_exact: true,
+    }
+  }
+}
+
+impl std::ops::Sub for Q {
+  type Output = Self;
+  fn sub(self, rhs: Self) -> Self::Output {
+    if rhs.eval() > self.eval() {
+      unimplemented!()
+    }
+    Self {
+      val: self.val - rhs.val,
+      m: self.m,
+      n: self.n,
+      is_exact: true,
+    }
+  }
+}
+
+impl std::ops::Mul for Q {
+  type Output = Self;
+  fn mul(self, rhs: Self) -> Self::Output {
+    Self {
+      val: self.val * rhs.val,
+      m: self.m + rhs.m,
+      n: self.n + rhs.n,
+      is_exact: true,
+    }
+  }
+}
+
+impl std::fmt::Debug for Q {
+  fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+    let ans = debug_print(self.val, self.m, self.m + self.n, self.is_exact);
+    write!(f, "{}", ans)
+  }
+}
+
+impl std::fmt::Display for Q {
+  fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+    let ans = format!("Q<{},{}>({})", self.m, self.n, self.val);
+    // ans = self.q_fmt();
+    write!(f, "{}", ans)
+  }
 }
 
 #[allow(non_snake_case)]
-pub fn to_Fx(x: f64, m: i32, b: i32, round: bool) -> Result<Fx, String> {
-    let fx_q = crate::to_fixed(x, m, b - m, round);
-    match fx_q {
-        Ok(fx) => Ok(Fx::new(fx.val, fx.m, fx.m + fx.n, fx.is_exact)),
-        Err(e) => Err(e.to_string()),
-    }
+pub fn to_Q(x: f64, m: i32, n: i32, round: bool) -> Result<Q, String> {
+  crate::to_fixed(x, m, n, round)
 }
```

### Comparing `fixed2float-3.0.0_rc1/local_dependencies/fixed2float/src/fixed_point.rs` & `fixed2float-4.0.0_rc1/local_dependencies/fixed2float/src/fixed_point.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,113 @@
 mod fx_fx;
 mod fx_q;
 use crate::UInt;
 pub use fx_fx::{to_Fx, Fx};
 pub use fx_q::{to_Q, Q};
 
 pub trait FixedPoint {
-    fn eval(&self) -> f64;
+  fn eval(&self) -> f64;
 }
 
 fn debug_print(val: UInt, m: i32, b: i32, is_exact: bool) -> String {
-    const ANSI_RESET_COLOR: &str = "\x1b[0m";
-    const ANSI_BLACK: &str = "\x1b[37;40m"; // bold, black background, white foreground
-    const ANSI_MAGENTA: &str = "\x1b[45m"; // non bold, magenta background, black foreground
+  const ANSI_RESET_COLOR: &str = "\x1b[0m";
+  const ANSI_RED: &str = "\x1b[37;41m";
+  const ANSI_BLACK: &str = "\x1b[37;40m"; // bold, black background, white foreground
+  const ANSI_MAGENTA: &str = "\x1b[45m"; // non bold, magenta background, black foreground
+
+  let bits = format!("{:0width$b}", val, width = (b) as usize);
+
+  let dots = if is_exact { "" } else { "..." };
+
+  let ans = format!(
+    "{ANSI_RED}{sign}{ANSI_MAGENTA}{int}{ANSI_BLACK}{frac}{dots}{ANSI_RESET_COLOR}",
+    sign = &bits[..1],
+    int = &bits[1..(m + 1) as usize],
+    frac = &bits[(m + 1) as usize..],
+  );
 
-    let bits = format!("{:0width$b}", val, width = (b) as usize);
-
-    let dots = if is_exact { "" } else { "..." };
-
-    let ans = format!(
-        "{ANSI_MAGENTA}{int}{ANSI_BLACK}{frac}{dots}{ANSI_RESET_COLOR}",
-        int = &bits[..m as usize],
-        frac = &bits[m as usize..],
-    );
-
-    ans
+  ans
 }
 
 #[cfg(test)]
 mod test {
 
-    use crate::fixed_point::Q;
+  use crate::fixed_point::{Fx, Q};
 
-    #[test]
-    fn test_add() {
-        let fx1 = Q::new(0b1111, 3, 1, true);
-        let fx2 = Q::new(0b1110, 3, 1, true);
-        let fx3 = Q::new(0b11101, 4, 1, true);
-        assert_eq!(fx1 + fx2, fx3);
-    }
-
-    #[test]
-    fn test_sub() {
-        let fx1 = Q::new(0b1111, 3, 1, true);
-        let fx2 = Q::new(0b1110, 3, 1, true);
-        let fx3 = Q::new(0b0001, 3, 1, true);
-        assert_eq!(fx1 - fx2, fx3);
-    }
-
-    #[test]
-    fn test_shift() {
-        let fx1 = Q::new(0b1111, 3, 1, true);
-        assert_eq!(fx1 << 1, Q::new(0b1110, 3, 1, true));
-        assert_eq!(fx1 << 2, Q::new(0b1100, 3, 1, true));
-        assert_eq!(fx1 << 3, Q::new(0b1000, 3, 1, true));
-        assert_eq!(fx1 >> 1, Q::new(0b0111, 3, 1, true));
-    }
-
-    // #[test]
-    // #[ignore]
-    // fn test_index_right_idx_0() {
-    //     let fx1 = Q::new(0b10010011, 6, 2, true); // 36.75
-    //     let size = (fx1.m + fx1.n) as usize;
-
-    //     assert_eq!(fx1.index(size..0).is_err(), true);
-    //     assert_eq!(fx1.index(size - 1..0), Ok(Q::new(0b10010011, 6, 2, true)));
-    //     assert_eq!(fx1.index(size - 2..0), Ok(Q::new(0b0010011, 5, 2, true)));
-    //     assert_eq!(fx1.index(size - 3..0), Ok(Q::new(0b010011, 4, 2, true)));
-    //     assert_eq!(fx1.index(size - 4..0), Ok(Q::new(0b10011, 3, 2, true)));
-    //     assert_eq!(fx1.index(size - 5..0), Ok(Q::new(0b0011, 2, 2, true)));
-    //     assert_eq!(fx1.index(size - 6..0), Ok(Q::new(0b011, 1, 2, true)));
-    //     assert_eq!(fx1.index(size - 7..0), Ok(Q::new(0b11, 0, 2, true)));
-
-    //     // assert_eq!(
-    //     //     fx1.index(size - 8..0),
-    //     //     Ok(Q::new(0b1, 0, 1, true))
-    //     // );
-
-    //     // assert_eq!(fx1.index(size - 9..0).is_err(), true);
-    // }
-
-    // #[test]
-    // #[ignore]
-    // fn test_index_left_idx_max() {
-    //     let fx1 = Q::new(0b10010011, 6, 2, true); // 36.75
-    //     let size = (fx1.m + fx1.n) as usize;
-
-    //     assert_eq!(fx1.index(size..0).is_err(), true);
-
-    //     assert_eq!(fx1.index(size - 1..0), Ok(Q::new(0b10010011, 6, 2, true)));
-
-    //     assert_eq!(fx1.index(size - 1..1), Ok(Q::new(0b1001001, 6, 1, true)));
-
-    //     assert_eq!(fx1.index(size - 1..2), Ok(Q::new(0b100100, 6, 0, true)));
-
-    //     assert_eq!(fx1.index(size - 1..3), Ok(Q::new(0b10010, 5, 0, true)));
-
-    //     assert_eq!(fx1.index(size - 1..4), Ok(Q::new(0b1001, 4, 0, true)));
-
-    //     assert_eq!(fx1.index(size - 1..5), Ok(Q::new(0b100, 3, 0, true)));
-
-    //     assert_eq!(fx1.index(size - 1..6), Ok(Q::new(0b10, 2, 0, true)));
-
-    //     // assert_eq!(
-    //     //     fx1.index(size-1..7),
-    //     //     Ok(Q::new(0b1, 1, 0, true))
-    //     // );
+  #[test]
+  fn test_add() {
+    let fx1 = Q::new(0b1111, 3, 1, true);
+    let fx2 = Q::new(0b1110, 3, 1, true);
+    let fx3 = Q::new(0b11101, 4, 1, true);
+    assert_eq!(fx1 + fx2, fx3);
+  }
+
+  #[test]
+  fn test_sub() {
+    let fx1 = Fx::new(0b0_111_1, 3, 5, true); // 7.5
+    let fx2 = Fx::new(0b0_111_0, 3, 5, true); // 7.0
+    let fx3 = Fx::new(0b0_000_1, 3, 5, true); // 0.5
+    assert_eq!(fx1 - fx2, fx3);
+  }
+
+  #[test]
+  fn test_shift() {
+    let fx1 = Q::new(0b1111, 3, 1, true);
+    assert_eq!(fx1 << 1, Q::new(0b1110, 3, 1, true));
+    assert_eq!(fx1 << 2, Q::new(0b1100, 3, 1, true));
+    assert_eq!(fx1 << 3, Q::new(0b1000, 3, 1, true));
+    assert_eq!(fx1 >> 1, Q::new(0b0111, 3, 1, true));
+  }
+
+  // #[test]
+  // #[ignore]
+  // fn test_index_right_idx_0() {
+  //     let fx1 = Q::new(0b10010011, 6, 2, true); // 36.75
+  //     let size = (fx1.m + fx1.n) as usize;
+
+  //     assert_eq!(fx1.index(size..0).is_err(), true);
+  //     assert_eq!(fx1.index(size - 1..0), Ok(Q::new(0b10010011, 6, 2, true)));
+  //     assert_eq!(fx1.index(size - 2..0), Ok(Q::new(0b0010011, 5, 2, true)));
+  //     assert_eq!(fx1.index(size - 3..0), Ok(Q::new(0b010011, 4, 2, true)));
+  //     assert_eq!(fx1.index(size - 4..0), Ok(Q::new(0b10011, 3, 2, true)));
+  //     assert_eq!(fx1.index(size - 5..0), Ok(Q::new(0b0011, 2, 2, true)));
+  //     assert_eq!(fx1.index(size - 6..0), Ok(Q::new(0b011, 1, 2, true)));
+  //     assert_eq!(fx1.index(size - 7..0), Ok(Q::new(0b11, 0, 2, true)));
+
+  //     // assert_eq!(
+  //     //     fx1.index(size - 8..0),
+  //     //     Ok(Q::new(0b1, 0, 1, true))
+  //     // );
+
+  //     // assert_eq!(fx1.index(size - 9..0).is_err(), true);
+  // }
+
+  // #[test]
+  // #[ignore]
+  // fn test_index_left_idx_max() {
+  //     let fx1 = Q::new(0b10010011, 6, 2, true); // 36.75
+  //     let size = (fx1.m + fx1.n) as usize;
+
+  //     assert_eq!(fx1.index(size..0).is_err(), true);
+
+  //     assert_eq!(fx1.index(size - 1..0), Ok(Q::new(0b10010011, 6, 2, true)));
+
+  //     assert_eq!(fx1.index(size - 1..1), Ok(Q::new(0b1001001, 6, 1, true)));
+
+  //     assert_eq!(fx1.index(size - 1..2), Ok(Q::new(0b100100, 6, 0, true)));
+
+  //     assert_eq!(fx1.index(size - 1..3), Ok(Q::new(0b10010, 5, 0, true)));
+
+  //     assert_eq!(fx1.index(size - 1..4), Ok(Q::new(0b1001, 4, 0, true)));
+
+  //     assert_eq!(fx1.index(size - 1..5), Ok(Q::new(0b100, 3, 0, true)));
+
+  //     assert_eq!(fx1.index(size - 1..6), Ok(Q::new(0b10, 2, 0, true)));
+
+  //     // assert_eq!(
+  //     //     fx1.index(size-1..7),
+  //     //     Ok(Q::new(0b1, 1, 0, true))
+  //     // );
 
-    //     assert_eq!(fx1.index(size - 8..8).is_err(), true);
-    // }
+  //     assert_eq!(fx1.index(size - 8..8).is_err(), true);
+  // }
 }
```

### Comparing `fixed2float-3.0.0_rc1/local_dependencies/fixed2float/src/lib.rs` & `fixed2float-4.0.0_rc1/local_dependencies/fixed2float/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -12,237 +12,280 @@
 
 const SIZE: u64 = 64;
 const MANT_SIZE: u64 = 52;
 const ES: u64 = 11;
 const EXP_BIAS: u64 = (1 << (ES - 1)) - 1;
 
 fn mask(size: u32) -> u128 {
-    match 1_u128.checked_shl(size) {
-        Some(v) => v - 1,
-        None => 0,
-    }
+  match 1_u128.checked_shl(size) {
+    Some(v) => v - 1,
+    None => 0,
+  }
+}
+
+fn sign(bits: u64) -> u64 {
+  bits >> (SIZE - 1)
 }
 
 fn exp(bits: u64) -> u64 {
-    ((bits & ((1 << (SIZE - 1)) - 1)) >> MANT_SIZE) & ((1 << MANT_SIZE) - 1)
+  ((bits & ((1 << (SIZE - 1)) - 1)) >> MANT_SIZE) & ((1 << MANT_SIZE) - 1)
 }
 
 fn mant(bits: u64) -> u64 {
-    bits & ((1 << MANT_SIZE) - 1)
+  bits & ((1 << MANT_SIZE) - 1)
 }
 
 /// Convert `x` (f64) into fixed point format (Qm.n), if possible.
 /// ```rust
 /// use fixed2float::{to_Q, Q};
+/// use fixed2float::to_fixed;
 /// assert_eq!(
 ///     to_Q(1.5, 1, 3, true),
 ///     Ok(
 ///         Q {
 ///             val: 0b1100,
 ///             m: 1,
 ///             n: 3,
 ///             is_exact: true,
 ///         }
 ///     )
 /// );
+/// assert_eq!(
+///     to_Q(-2.5, 3, 3, true),
+///     Ok(
+///         Q {
+///             val: 0b1101100,
+///             m: 3,
+///             n: 3,
+///             is_exact: true,
+///         }
+///     )
+/// );
 /// assert_eq!(to_Q(1.5, 1, 3, true).unwrap().val, 0b1100);
 /// assert_eq!(to_Q(0.0, 1, 5, true).unwrap().val, 0);
 /// assert_eq!(to_Q(1.5, 1, 3, true).unwrap().is_exact, true);
+///
+/// assert_eq!(to_fixed(-2.5, 3, 3, false).unwrap().val, 108);
 /// ```
-fn to_fixed(x: f64, m: i32, n: i32, round: bool) -> Result<Q, String> {
-    if x == 0.0 {
-        return Ok(Q {
-            val: 0,
-            m,
-            n,
-            is_exact: true,
-        });
-    }
-
-    let f64_bits = x.to_bits();
-
-    let exp = exp(f64_bits) as i32 - EXP_BIAS as i32;
-
-    let mant_plus_one = (1 << MANT_SIZE) | mant(f64_bits); // Q1.MANT_SIZE
-
-    let bits = mant_plus_one; // bits is mant_plus_one. the only thing that changes
-                              // is where _you_ interpret the point to be, which depends on `exp` at this point.
-                              // now all you have to do is slice out the fractional and non-fractional parts individually.
-
-    let fractional_part = bits as UInt & mask((MANT_SIZE as i32 - exp as i32) as u32) as UInt;
-    let integer_part = bits
-        .checked_shr((MANT_SIZE as i32 - exp as i32) as u32)
-        .unwrap_or(0);
-
-    // now, depending on `m` and `n` you need to figure out whether rouding occurs.
-    // if that's the case, that information is reported back to the user via the `is_exact` flag.
-    // whereas if the integer part does not fit into `m` bits you return the Err variant instead.
-
-    let integer_part_on_m_bits = integer_part as UInt & mask(m as u32) as UInt;
-
-    let mut fractional_part_on_n_bits = match (MANT_SIZE as i32 - exp as i32 - n as i32) >= 0 {
-        true => {
-            (fractional_part >> (MANT_SIZE as i32 - exp as i32 - n as i32) as u32)
-                & (mask(n as u32) as UInt)
-        }
-        _ => {
-            (fractional_part << (-(MANT_SIZE as i32 - exp as i32 - n as i32)))
-                & (mask(n as u32) as UInt)
-        }
-    };
-
-    if integer_part_on_m_bits < integer_part as UInt {
-        return Err(format!(
-            "Error: Integer field does not fit into `m` = {} bits.",
-            m
-        ));
-    }
-
-    let _len = (MANT_SIZE as i32 - exp as i32) - (n as i32 + 1);
-    let round_bit = match _len >= 0 {
-        true => fractional_part >> (_len) & 1 != 0,
-        _ => fractional_part.checked_shl(-_len as u32).unwrap_or(0) != 0,
-    };
+pub fn to_fixed(x: f64, m: i32, n: i32, round: bool) -> Result<Q, String> {
+  let f64_bits = x.to_bits();
 
-    if round && round_bit {
-        fractional_part_on_n_bits += 1;
-    }
-
-    let sticky_bit = match (MANT_SIZE as i32 - exp as i32 - n as i32) >= 0 {
-        true => {
-            fractional_part & mask((MANT_SIZE as i32 - exp as i32 - n as i32) as u32) as UInt != 0
-        }
-        _ => false,
-    };
+  let sign = sign(f64_bits);
 
-    let is_exact = !sticky_bit && !round_bit;
-    let ans = ((integer_part_on_m_bits) << n) + fractional_part_on_n_bits;
-    Ok(Q {
-        val: ans,
-        m,
-        n,
-        is_exact,
-    })
+  if x.abs() == 0.0 {
+    return Ok(Q {
+      val: (sign << (m + n)) as UInt,
+      m,
+      n,
+      is_exact: true,
+    });
+  }
+
+  let exp = exp(f64_bits) as i32 - EXP_BIAS as i32;
+
+  let mant_plus_one = (1 << MANT_SIZE) | mant(f64_bits); // Q1.MANT_SIZE
+
+  let bits = mant_plus_one; // bits is mant_plus_one. the only thing that changes
+                            // is where _you_ interpret the point to be, which depends on `exp` at this point.
+                            // now all you have to do is slice out the fractional and non-fractional parts individually.
+
+  let fractional_part = bits as UInt & mask((MANT_SIZE as i32 - exp) as u32) as UInt;
+  let integer_part = bits
+    .checked_shr((MANT_SIZE as i32 - exp) as u32)
+    .unwrap_or(0);
+
+  // now, depending on `m` and `n` you need to figure out whether rouding occurs.
+  // if that's the case, that information is reported back to the user via the `is_exact` flag.
+  // whereas if the integer part does not fit into `m` bits you return the Err variant instead.
+
+  let integer_part_on_m_bits = integer_part as UInt & mask(m as u32) as UInt;
+
+  let mut fractional_part_on_n_bits = match (MANT_SIZE as i32 - exp - n) >= 0 {
+    true => (fractional_part >> (MANT_SIZE as i32 - exp - n) as u32) & (mask(n as u32) as UInt),
+    _ => (fractional_part << (-(MANT_SIZE as i32 - exp - n))) & (mask(n as u32) as UInt),
+  };
+
+  if integer_part_on_m_bits < integer_part as UInt {
+    return Err(format!(
+      "Error: Integer field does not fit into `m` = {} bits.",
+      m
+    ));
+  }
+
+  let _len = (MANT_SIZE as i32 - exp) - (n + 1);
+  let round_bit = match _len >= 0 {
+    true => fractional_part >> (_len) & 1 != 0,
+    _ => fractional_part.checked_shl(-_len as u32).unwrap_or(0) != 0,
+  };
+
+  if round && round_bit {
+    fractional_part_on_n_bits += 1;
+  }
+
+  let sticky_bit = match (MANT_SIZE as i32 - exp - n) >= 0 {
+    true => fractional_part & mask((MANT_SIZE as i32 - exp - n) as u32) as UInt != 0,
+    _ => false,
+  };
+
+  let is_exact = !sticky_bit && !round_bit;
+  let ans_signless = ((integer_part_on_m_bits) << n) + fractional_part_on_n_bits;
+
+  let ans = match sign == 0 {
+    true => ans_signless,
+    false => (!ans_signless + 1 as UInt) & mask((m + n + 1) as u32),
+  };
+
+  Ok(Q {
+    val: ans,
+    m,
+    n,
+    is_exact,
+  })
 }
 
+#[deprecated(since="0.4.0")]
 /// Compute the real value represented by `bits` (str).
 /// ```rust
 /// use fixed2float::to_float_str;
-/// assert_eq!(to_float_str("00010011000000100001", 12, 8), Ok(304.12890625));
+/// assert_eq!(to_float_str("00010011000000100001", 12, 20), Ok(304.12890625));
 /// ```
-pub fn to_float_str(bits: &str, m: i32, n: i32) -> Result<f64, String> {
-    let bits_size = bits.len() as i32;
-    if bits_size != m + n {
-        return Err(format!(
-            "`bits` size  does not match the `m` + `n` size you specified. {} != {}",
-            bits_size,
-            m + n
-        ));
-    }
-
-    let mut ans = 0.0;
-
-    for i in (1..=n).rev() {
-        let bit = bits
-            .chars()
-            .nth(((m - 1 + i) as u16).into())
-            .unwrap()
-            .to_digit(2)
-            .unwrap(); //. parse::<i32>().unwrap();
-        ans += bit as f64 / (1 << i) as f64;
-    }
-
-    for i in 0..m {
-        let bit = bits
-            .chars()
-            .nth(((m - 1 - i) as u16).into())
-            .unwrap()
-            .to_digit(2)
-            .unwrap();
-        ans += bit as f64 * (1 << i) as f64;
-    }
+pub fn to_float_str(bits: &str, m: i32, b: i32) -> Result<f64, String> {
+  let n = b - m;
+  let bits_size = bits.len() as i32;
+  if bits_size != m + n {
+    return Err(format!(
+      "`bits` size  does not match the `m` + `n` size you specified. {} != {}",
+      bits_size,
+      m + n
+    ));
+  }
+
+  let mut ans = 0.0;
+
+  for i in (1..=n).rev() {
+    let bit = bits
+      .chars()
+      .nth(((m - 1 + i) as u16).into())
+      .unwrap()
+      .to_digit(2)
+      .unwrap(); //. parse::<i32>().unwrap();
+    ans += bit as f64 / (1 << i) as f64;
+  }
+
+  for i in 0..m {
+    let bit = bits
+      .chars()
+      .nth(((m - 1 - i) as u16).into())
+      .unwrap()
+      .to_digit(2)
+      .unwrap();
+    ans += bit as f64 * (1 << i) as f64;
+  }
 
-    Ok(ans)
+  Ok(ans)
 }
 
 /// Compute the real value represented by `bits`.
 /// ```rust
 /// use fixed2float::to_float;
-/// assert_eq!(to_float(0x13021, 20, 12, 8), Ok(304.12890625));
+/// assert_eq!(to_float(0b0_000100110000_00100001, 21, 12, 8), Ok(304.12890625));
 /// ```
-pub fn to_float(mut bits: UInt, size: i32, m: i32, n: i32) -> Result<f64, String> {
-    if size != m + n {
-        return Err(format!(
-            "`bits` size  does not match the `m` + `n` size you specified. {} != {}",
-            size,
-            m + n
-        ));
-    }
-
-    let mut ans = 0.0;
-
-    for i in (1..=n).rev() {
-        ans += match 2_i128.checked_pow(i as u32) {
-            None => 0.0,
-            Some(v) => (bits & 1) as f64 / v as f64,
-        };
-
-        //2_i128.pow (i as u32) as f64; //  (1 << i) as f64;
-        bits >>= 1;
-    }
-    for i in 0..m {
-        ans += (bits & 1) as f64 * 2_i128.pow(i as u32) as f64; // (1 << i) as f64;
-        bits >>= 1;
-    }
+pub fn to_float(bits: UInt, size: i32, m: i32, n: i32) -> Result<f64, String> {
+  if size != m + n + 1 {
+    return Err(format!(
+      "`bits` size  does not match the (`m` + `n` + 1) size you specified. {} != {}",
+      size,
+      m + n + 1
+    ));
+  }
+
+  let sign = (bits >> (m + n)) as u32;
+
+  let mut bits = match sign == 0 {
+    true => bits,
+    false => (!bits + 1) & mask(size as u32),
+  };
+
+  let mut ans = 0.0;
+
+  for i in (1..=n).rev() {
+    ans += match 2_i128.checked_pow(i as u32) {
+      None => 0.0,
+      Some(v) => (bits & 1) as f64 / v as f64,
+    };
+
+    //2_i128.pow (i as u32) as f64; //  (1 << i) as f64;
+    bits >>= 1;
+  }
+  for i in 0..m {
+    ans += (bits & 1) as f64 * 2_i128.pow(i as u32) as f64; // (1 << i) as f64;
+    bits >>= 1;
+  }
+
+  let ans = match sign == 0 {
+    true => ans,
+    false => -ans,
+  };
 
-    Ok(ans)
+  Ok(ans)
 }
 
 #[cfg(test)]
 mod tests {
-    use super::{to_fixed, to_float, to_float_str};
+  use super::{to_fixed, to_float, to_float_str};
 
-    #[test]
-    fn test_to_float() {
-        assert_eq!(to_float(0b1010000010110000, 16, 1, 15), Ok(1.25537109375));
-        assert_eq!(to_float(0b1010000010110000, 16, 1, 14).is_err(), true);
-        assert_eq!(to_float(0b1010000010110000, 16, 1, 15).is_err(), false);
-        assert_eq!(to_float(0b1010000010110000, 16, 1, 16).is_err(), true);
-        assert_eq!(to_float_str("1010000010110000", 1, 15), Ok(1.25537109375));
-        assert_eq!(to_float_str("1010000010110000", 1, 14).is_err(), true);
-        assert_eq!(to_float_str("1010000010110000", 1, 15).is_err(), false);
-        assert_eq!(to_float_str("1010000010110000", 1, 16).is_err(), true);
-    }
-
-    #[test]
-    fn test_to_fixed() {
-        use super::fixed_point::Q;
-
-        assert_eq!(to_fixed(10.25, 4, 3, true), Ok(Q::new(82, 4, 3, true)));
-        assert_eq!(to_fixed(10.25, 3, 3, true).is_err(), true);
-        assert_eq!(to_fixed(10.25, 8, 3, true), Ok(Q::new(82, 8, 3, true)));
-        assert_eq!(to_fixed(10.25, 8, 2, true), Ok(Q::new(41, 8, 2, true)));
-        assert_eq!(to_fixed(10.25, 8, 1, true), Ok(Q::new(21, 8, 1, false)));
-        assert_eq!(to_fixed(10.25, 8, 0, true), Ok(Q::new(10, 8, 0, false)));
-        assert_eq!(to_fixed(0.0078125, 1, 1, true), Ok(Q::new(0, 1, 1, false)));
-        assert_eq!(to_fixed(0.0078125, 1, 2, true), Ok(Q::new(0, 1, 2, false)));
-        assert_eq!(to_fixed(0.0078125, 1, 3, true), Ok(Q::new(0, 1, 3, false)));
-        assert_eq!(to_fixed(0.0078125, 1, 4, true), Ok(Q::new(0, 1, 4, false)));
-        assert_eq!(to_fixed(0.0078125, 1, 5, true), Ok(Q::new(0, 1, 5, false)));
-        assert_eq!(to_fixed(0.0078125, 1, 6, true), Ok(Q::new(1, 1, 6, false)));
-        assert_eq!(to_fixed(0.0078125, 1, 7, true), Ok(Q::new(1, 1, 7, true)));
-        assert_eq!(to_fixed(0.0078125, 1, 8, true), Ok(Q::new(2, 1, 8, true)));
-        assert_eq!(to_fixed(0.0078125, 1, 9, true), Ok(Q::new(4, 1, 9, true)));
-        assert_eq!(to_fixed(1.387, 2, 15, true).unwrap().val, 45449);
-        assert_eq!(to_fixed(4.3, 2, 15, true).is_err(), true);
-    }
-
-    #[test]
-    fn back_and_forth() {
-        let x = 10.25;
-        let (m, n) = (21, 3);
-        assert_eq!(
-            to_float(to_fixed(x, m, n, true).unwrap().val, 24, m, n).unwrap(),
-            x
-        );
-    }
+  #[test]
+  fn test_to_float() {
+    assert_eq!(to_float(0b01010000010110000, 17, 1, 15), Ok(1.25537109375));
+    assert_eq!(to_float(0b01010000010110000, 17, 1, 14).is_err(), true);
+    assert_eq!(to_float(0b01010000010110000, 17, 1, 15).is_err(), false);
+    assert_eq!(to_float(0b01010000010110000, 17, 1, 16).is_err(), true);
+    // assert_eq!(to_float_str("1010000010110000", 1, 16), Ok(1.25537109375));
+    // assert_eq!(to_float_str("1010000010110000", 1, 15).is_err(), true);
+    // assert_eq!(to_float_str("1010000010110000", 1, 16).is_err(), false);
+    // assert_eq!(to_float_str("1010000010110000", 1, 17).is_err(), true);
+  }
+
+  #[test]
+  fn test_to_fixed() {
+    use super::fixed_point::Q;
+
+    // assert_eq!(to_fixed(10.25, 4, 3, true), Ok(Q::new(82, 4, 3, true)));
+    // assert_eq!(to_fixed(10.25, 3, 3, true).is_err(), true);
+    // assert_eq!(to_fixed(10.25, 8, 3, true), Ok(Q::new(82, 8, 3, true)));
+    // assert_eq!(to_fixed(10.25, 8, 2, true), Ok(Q::new(41, 8, 2, true)));
+    // assert_eq!(to_fixed(10.25, 8, 1, true), Ok(Q::new(21, 8, 1, false)));
+    // assert_eq!(to_fixed(10.25, 8, 0, true), Ok(Q::new(10, 8, 0, false)));
+    // assert_eq!(to_fixed(0.0078125, 1, 1, true), Ok(Q::new(0, 1, 1, false)));
+    // assert_eq!(to_fixed(0.0078125, 1, 2, true), Ok(Q::new(0, 1, 2, false)));
+    // assert_eq!(to_fixed(0.0078125, 1, 3, true), Ok(Q::new(0, 1, 3, false)));
+    // assert_eq!(to_fixed(0.0078125, 1, 4, true), Ok(Q::new(0, 1, 4, false)));
+    // assert_eq!(to_fixed(0.0078125, 1, 5, true), Ok(Q::new(0, 1, 5, false)));
+    // assert_eq!(to_fixed(0.0078125, 1, 6, true), Ok(Q::new(1, 1, 6, false)));
+    // assert_eq!(to_fixed(0.0078125, 1, 7, true), Ok(Q::new(1, 1, 7, true)));
+    // assert_eq!(to_fixed(0.0078125, 1, 8, true), Ok(Q::new(2, 1, 8, true)));
+    // assert_eq!(to_fixed(0.0078125, 1, 9, true), Ok(Q::new(4, 1, 9, true)));
+    // assert_eq!(to_fixed(1.387, 2, 15, true).unwrap().val, 45449);
+    // assert_eq!(to_fixed(4.3, 2, 15, true).is_err(), true);
+
+    assert_eq!(to_fixed(4.0, 4, 2, false).unwrap().val, 0b0_0100_00);
+    assert_eq!(to_fixed(-4.0, 4, 2, false).unwrap().val, 0b1_1100_00);
+    assert_eq!(to_fixed(8.75, 4, 2, false).unwrap().val, 0b0_1000_11);
+    assert_eq!(to_fixed(9.5, 4, 2, false).unwrap().val, 0b0_1001_10);
+    assert_eq!(to_fixed(15.75, 4, 2, false).unwrap().val, 0b0_1111_11);
+    assert_eq!(to_fixed(15.8, 4, 2, false).unwrap().val, 0b0_1111_11);
+    assert_eq!(to_fixed(16.0, 4, 2, false).is_err(), true);
+    assert_eq!(to_fixed(0.0, 2, 1, false).unwrap().val, 0b0_00_0);
+    assert_eq!(to_fixed(-0.0, 2, 1, false).unwrap().val, 0b1_00_0);
+  }
+
+  #[test]
+  fn back_and_forth() {
+    // 0_1_010
+    let x = 1.25;
+    let (m, n) = (1, 3);
+    assert_eq!(
+      to_float(to_fixed(x, m, n, false).unwrap().val, 5, m, n).unwrap(),
+      x
+    );
+  }
 }
```

### Comparing `fixed2float-3.0.0_rc1/Cargo.toml` & `fixed2float-4.0.0_rc1/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-fixed2float"
-version = "3.0.0-rc1"
+version = "4.0.0-rc1"
 authors = ["Francesco Urbani <francescourbanidue@gmail.com>"]
 edition = "2021"
 keywords = ["fixed", "float", "q-format"]
 documentation = ""
 # homepage = ""
 readme = "README.md"
 repository = "https://github.com/urbanij/fixed2float"
@@ -23,8 +23,8 @@
 
 [package.metadata.maturin]
 name = "fixed2float"
 
 
 [dependencies]
 fixed2float = { path = "local_dependencies/fixed2float" }
-pyo3 = { version = "0.15.1", features = ["extension-module"], optional = false }
+pyo3 = { version = "0.18.2", features = ["extension-module"], optional = false }
```

### Comparing `fixed2float-3.0.0_rc1/Makefile` & `fixed2float-4.0.0_rc1/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	# cargo build --release
 	# cp $(CARGO_TARGET_DIR)/release/libfixed2float.$(EXT) fixed2float/fixed2float.so
 
 build: pre-commit
 	maturin build
 	
 install:
-	pip install --force-reinstall $(CARGO_TARGET_DIR)/wheels/fixed2float-*cp310-*.whl
+	pip install --force-reinstall $(CARGO_TARGET_DIR)/wheels/fixed2float-*.whl
 	
 
 pre-commit:
 	cargo fmt
 	cargo test
 
 demo:
```

### Comparing `fixed2float-3.0.0_rc1/examples/example.py` & `fixed2float-4.0.0_rc1/examples/example.py`

 * *Files identical despite different names*

### Comparing `fixed2float-3.0.0_rc1/pyproject.toml` & `fixed2float-4.0.0_rc1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -23,7 +23,10 @@
 # files = ["fixed2float", "tests"]
 
 [[tool.mypy.overrides]]
 
 
 [tool.coverage.report]
 # exclude_lines = ["pragma: no cover", "@overload"]
+
+[tool.maturin]
+name = "fixed2float"
```

