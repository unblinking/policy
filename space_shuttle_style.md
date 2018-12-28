# Space Shuttle Style  

Whenever it is not detrimental, follow the Kubernetes "Space Shuttle Style" of overly verbose, commented, and branchy code.  

Stolen from [kubernetes/kubernetes](https://github.com/kubernetes/kubernetes/blob/ec2e767e59395376fa191d7c56a74f53936b7653/pkg/controller/volume/persistentvolume/pv_controller.go)  

```
// ==================================================================
// PLEASE DO NOT ATTEMPT TO SIMPLIFY THIS CODE.
// KEEP THE SPACE SHUTTLE FLYING.
// ==================================================================
//
// This controller is intentionally written in a very verbose style.  You will
// notice:
//
// 1.  Every 'if' statement has a matching 'else' (exception: simple error
//     checks for a client API call)
// 2.  Things that may seem obvious are commented explicitly
//
// We call this style 'space shuttle style'.  Space shuttle style is meant to
// ensure that every branch and condition is considered and accounted for -
// the same way code is written at NASA for applications like the space
// shuttle.
//
// Originally, the work of this controller was split amongst three
// controllers.  This controller is the result a large effort to simplify the
// PV subsystem.  During that effort, it became clear that we needed to ensure
// that every single condition was handled and accounted for in the code, even
// if it resulted in no-op code branches.
//
// As a result, the controller code may seem overly verbose, commented, and
// 'branchy'.  However, a large amount of business knowledge and context is
// recorded here in order to ensure that future maintainers can correctly
// reason through the complexities of the binding behavior.  For that reason,
// changes to this file should preserve and add to the space shuttle style.
//
// ==================================================================
// PLEASE DO NOT ATTEMPT TO SIMPLIFY THIS CODE.
// KEEP THE SPACE SHUTTLE FLYING.
// ==================================================================
```

