# blocgen [WIP]

>NOTE:
>This script is heavily Work In Progreess

Generate BLoC and Cubit boilerplate easily with a cli tool

This generates a bloc or cubit folder in your current directory according to the argument provided

## Installation

```bash
git clone https://github.com/edr3x/blocgen
cd blocgen
sudo cp blocgen /usr/local/bin/
cd .. && sudo rm -rf blocgen
```

## Instructions
>Note:\
>Since this generates folder in your present working directory so you have to be in the appropriate directory before you execute the command

### To generate BLoC

```sh
blocgen -b <name>
```

- Example:
```sh
blocgen -b get_user_details
```

This will generate

```
get_user_details_bloc/
|
|___ get_user_details_bloc.dart
|
|___ get_user_details_event.dart
|
|___ get_user_details_state.dart
```

with appropriate snippets with respect to file

### To generate Cubit

```sh
blocgen -c <name>
```

- Example:
```sh
blocgen -c get_user_details
```

This will generate

```
get_user_details_cubit/
|
|___ get_user_details_cubit.dart
|
|___ get_user_details_state.dart
```

with appropriate snippets with respect to file

>Note:\
>name must be in snakecase i.e. `user_details`

### Help

```sh
blocgen -h
```
