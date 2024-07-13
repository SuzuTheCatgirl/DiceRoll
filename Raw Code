All the code contained in DiceRoll.exe

extern crate rand;
use rand::Rng;
use std::io;
use std::io::prelude::*;

fn pause() {
    let mut stdin = io::stdin();
    let mut stdout = io::stdout();
    write!(stdout, "Press Enter to close.").unwrap();
    stdout.flush().unwrap();
    let _ = stdin.read(&mut [0u8]).unwrap();
}

fn main() {
    let mut rng = rand::thread_rng();
    let n: u32 = rng.gen_range(1..10);
    let m: u32 = rng.gen_range(1..10);
    let nm: u32 = n+m;
    println!("Roll: {}", n);
    println!("Roll: {}", m);
    println!("Full Roll: {}", nm);
    if n==1 || m==1 {println!("Disadvantage...")}
    else if n==m {println!("Advantage Roll!")};
    if nm>=18 && nm<=20 {println!("Critical Hit!!")};
    if nm>=2 && nm<=6 {println!("Critical Miss..")};
    pause();

}
