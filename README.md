# Rust HDC2080 Low-Power Humidity and Temperature Digital Sensor Driver

[![crates.io](https://img.shields.io/crates/v/hdc2080.svg)](https://crates.io/crates/hdc2080)
[![Docs](https://docs.rs/hdc2080/badge.svg)](https://docs.rs/hdc2080)
[![Build Status](https://travis-ci.com/eldruin/hdc2080-rs.svg?branch=master)](https://travis-ci.com/eldruin/hdc2080-rs)
[![Coverage Status](https://coveralls.io/repos/github/eldruin/hdc2080-rs/badge.svg?branch=master)](https://coveralls.io/github/eldruin/hdc2080-rs?branch=master)

This is a platform agnostic Rust driver for the HDC2080 low-power humidity and
temperature digital sensor using the [`embedded-hal`] traits.

This driver allows you to:
- Set the measurement mode. Temperature only or temperature and humidity. See: `set_measurement_mode()`.
- Make one shot measurement. See: `read()`.
- Read the data and interrupt status. See: `status()`.
- Trigger a software reset. See: `software_reset()`.
- Read the manufacturer ID. See: `manufacturer_id()`.
- Read the device ID. See: `device_id()`.

<!-- TODO
[Introductory blog post]()
-->

The HDC2080 device is an integrated humidity and temperature sensor that
provides high accuracy measurements with very low power consumption in a
small DFN package. The capacitive-based sensor includes new integrated
digital features and a heating element to dissipate condensation and moisture.

The HDC2080 digital features include programmable interrupt thresholds to
provide alerts and system wake-ups without requiring a microcontroller to
be continuously monitoring the system. Combined with programmable sampling
intervals, a low power consumption, and a support for a 1.8-V supply voltage,
the HDC2080 is designed for battery-operated systems.

This driver is compatible with HDC2080, HDC2021 and HDC2010.

Datasheets: [HDC2080](https://www.ti.com/lit/ds/symlink/hdc2080.pdf), [HDC2021](https://www.ti.com/lit/ds/symlink/hdc2021.pdf), [HDC2010](https://www.ti.com/lit/ds/symlink/hdc2010.pdf)

<!-- TODO
## Usage

To use this driver, import this crate and an `embedded_hal` implementation,
then instantiate the device.

Please find additional examples using hardware in this repository: [driver-examples]

[driver-examples]: https://github.com/eldruin/driver-examples

```rust
```
-->
## Support

For questions, issues, feature requests, and other changes, please file an
[issue in the github project](https://github.com/eldruin/hdc2080-rs/issues).

## License

Licensed under either of

 * Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or
   http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or
   http://opensource.org/licenses/MIT)

at your option.

### Contributing

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall
be dual licensed as above, without any additional terms or conditions.

[`embedded-hal`]: https://github.com/rust-embedded/embedded-hal