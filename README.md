# PHP array_merge() Unexpected Behavior with Numeric Keys

This repository demonstrates a subtle but important quirk in PHP's `array_merge()` function when dealing with numeric keys.  When merging arrays with overlapping numeric keys, `array_merge()` overwrites values from the first array with those from the subsequent arrays, rather than appending them. This is counter-intuitive and can lead to data loss if not carefully considered.

The `bug.php` file showcases this unexpected behavior. The `bugSolution.php` provides a solution using `array_push()` or `+` operator to correctly append array elements.

This is a common pitfall for developers unfamiliar with this specific aspect of `array_merge()`'s functionality.  The provided solution offers a safer alternative to avoid data loss.