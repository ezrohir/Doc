
## Subscripttion
A ***subscriber*** is anything that is waiting or capable of waiting for events from a `signal`.

A subscription is created through any call to -subscribeNext:error:completed:, or one of the corresponding convenience methods. Technically, most RACStream and RACSignal operators create subscriptions as well, but these intermediate subscriptions are usually an implementation detail.

## Subjects
A subject, represented by the RACSubject class, is a signal that can be manually controlled.

Subjects can be thought of as the "mutable" variant of a signal, much like NSMutableArray is for NSArray. They are extremely useful for bridging non-RAC code into the world of signals.
