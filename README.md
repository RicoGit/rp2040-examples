
used project template - https://github.com/rp-rs/rp2040-project-templ


// A basic rp2040-hal project with blinky and rtt logging example code. With this you can quickly get started on a new rp2040 project  

    cargo generate \
    --git https://github.com/rp-rs/rp2040-project-template \
    --branch main \
    --name rp2040-examples
            
Install

    sudo apt-get install -y  libudev-dev

    rustup target install thumbv6m-none-eabi

    cargo install flip-link
    cargo install probe-rs --features=cli --locked

    cargo install elf2uf2-rs --locked

Then just run 

    cargo run --release
    
This build elf file, convert it to uf2 and send to Pico flash drive.

If you see "Unable to find mounted pico" - press boot btn and plug Pico to usb.

see this instruction for more info - https://github.com/rp-rs/rp-hal#loading-a-uf2-over-usb


