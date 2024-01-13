# Norwegian Dvorak layout
for use when pc is set to Norwegian QWERTY layout, keyboard has keys moved to a "physical" dvorak layout.

# tips:
create a keymap in the qmk_firmware source based on the default:
`cp -r ~/qmk_firmware/keyboards/omkbd/ergodash/rev1/keymaps/default ~/qmk_firmware/keyboards/omkbd/ergodash/rev1/keymaps/tc`
convert json to keympap.c with:
`qmk json2c keymap.json > ~/qmk_firmware/keyboards/omkbd/ergodash/rev1/keymaps/tc/keymap.c`
compile to check:
`qmk compile -kb omkbd/ergodash/rev1 -km tc`
flash to use:
`qmk flash -kb omkbd/ergodash/rev1 -km tc`
