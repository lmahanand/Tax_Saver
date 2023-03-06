# Tax_Saver
A cross platform mobile app that connects to a users bank transaction history and analyzes which potential tax savings could be made into a report.

# Dependencies
- [Flutter](https://docs.flutter.dev/)
- [Android Studio] (https://developer.android.com/studio)
- [Xcode for iOS] (https://developer.apple.com/xcode/)

## Setup & Installation
-------------------------------------------------

#### Step 1: Install Flutter

Flutter is an open source framework by Google for building natively compiled, multi-platform applications from a single codebase. That could be iOS, Android, Web, MacOS, Linux, & more. In this example, we're just going to focus on mobile platforms (iOS & Android) Flutter uses a language called Dart, which compiles down to native Swift and Java, for iOS and Android respectively. The best way to learn Flutter is to complete steps 1-3 of the official Flutter beginner tutorial. You'll need dependencies for each platform you'd like to push to, so in our case that means Xcode & Android Studio.

[Install  Link ](https://docs.flutter.dev/get-started/install)

#### Step 2: Install Android Strudio

Install android studio by referring the [link] (https://developer.android.com/studio)

#### Step 3: Install xcode

Refer this [link] (https://www.freecodecamp.org/news/install-xcode-command-line-tools/)

#### Step 4: Download and run this code

Download the code with the following command in a command-line interface on your operating system of choice:

`` 
git clone https://github.com/lmahanand/Tax_Saver.git
`` 

then enter the examples repository:

`` 
cd Tax_Saver/examples
``

and install all dependencies from the pubspec.yaml file with the following command:

`` 
flutter pub get
``

*and add your test user/pass to the users.dart file!*

Lastly, run the app with this command:

`` 
flutter run
``

#### Step 5: Add Plaid to get transaction history

[Plaid](https://plaid.com/) provides developers with tools to connect users  financial institutions to apps they love. Go to Plaid.com and signup to get an API key. Then integrate it with [this](https://github.com/jorgefspereira/plaid_flutter) plugin titled plaid-flutter. You'll need to generate a link token. I just curl'd it from command line and pasted it into the app to get Plaid's Link View to show up.

Find detailed instructions [here](https://dashboard.plaid.com/overview/sandbox)

Plaid example code to start Plaid Login

```Dart

 final configuration = LinkTokenConfiguration(
                    token: 'link-sandbox-YOURCODE');
                await PlaidLink.open(configuration: configuration);
```
