# Mood Tracker

This Rust program is a simple mood and productivity tracker, meant to be run from the command line. 

It prompts the user to enter their current mood, the number of work tasks completed, and whether they exercised. 

It provides feedback based on the user's input and appends this information, along with a timestamp, to a log file in the current directory.

The code is in [main.rs](https://github.com/julianeon/moodtracker/blob/main/src/main.rs) and an example log file, with multiple appends, is shown in [file_10_24_23.txt](https://github.com/julianeon/moodtracker/blob/main/src/file_10_24_23.txt).

While [main.rs](https://github.com/julianeon/moodtracker/blob/main/src/main.rs) is implemented with traits, if you want to see the code without traits, view [main_without_traits.rs](https://github.com/julianeon/moodtracker/blob/main/src/main_without_traits.rs), which may be easier to understand if you are new to Rust.

## Features 

### 1. Strong Typing
Rust enforces strong typing, ensuring that variables have clear and consistent data types. In this code, the use of structs for `Mood`, `Exercise` and `WorkCompleted` provides clear and strict typing for mood, exercise status, and work task counts.

### 2. Memory Safety
Rust's ownership and borrowing system allows for safe concurrent programming. It ensures that shared data is accessed safely, reducing the risk of data corruption or race conditions.

### 3. Pattern Matching
Rust's pattern matching elegantly handles the user input. The user input is matched against specific patterns in the `prompt_user` methods, making the code more readable and simpler to understand.

### 4. Error Handling
Rust encourages robust error handling through the use of the `Result` type in the `append_string_to_file` function. It ensures that errors are explicitly handled, unlike scripting languages where errors might be more difficult to trace.

For a longer take on Rust's advantages, see this [blog post](https://www.rerun.io/blog/why-rust).

## Usage

1. Clone this repository to your local machine.

2. Make sure you have Rust installed. If not, you can install it from [Rust's official website](https://www.rust-lang.org/tools/install).

3. Open a terminal and navigate to the project directory.

4. Compile and run the program using the following command:

   ```shell
   cargo run
   ```

5. Follow the prompts to enter your mood, the number of work tasks completed, and whether you exercised.

6. The program will display feedback based on your input, and the feedback, along with a timestamp, will be appended to a daily log file.

## License

This code is provided under the [MIT License](LICENSE). Feel free to use and modify it as needed for your own purposes.

