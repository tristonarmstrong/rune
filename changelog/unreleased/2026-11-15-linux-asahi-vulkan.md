- **Linux: an app on Apple silicon uses Asahi's Vulkan driver.** Asahi's Honeykrisp reports Vulkan
  conformance version 0, and wgpu hides adapters that report none unless the instance allows
  nonconformant adapters, so an app built on Rune found no GPU adapter on Apple silicon Linux. The
  instance now allows them. On a machine with a conformant adapter too, Rune's pick still chooses
  the compositor's GPU first, so the conformant one is unaffected.
