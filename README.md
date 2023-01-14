# KeyboardManager

KeyboardManager

This project is only for SwiftUI

When View uses ignoresSafeArea or edgesIgnoringSafeArea(.bottom)

this framework can be used because TextField and TextEditor cannot make the keyboard bounce

Encapsulated UITextView, UITextField can also be used
Supported Platforms

    iOS 13.0
    macOS 10.15
    tvOS 13.0
    watchOS 6.0

Usage

    @State private var text: String = ""
    
    var body: some View {
        VStack {
            Spacer()
            KeyboardHost {
                TextField("please enter text", text: $text)
                    .frame(width: 200, height: 40, alignment: .center)
                    .padding(.bottom, 20)
            }
        }
        .ignoresSafeArea()
    }

Installation

You can add KeyboardHost to an Xcode project by adding it as a package dependency.

    From the File menu, select Swift Packages › Add Package Dependency…
    Enter https://github.com/mrsafadi2/KeyboardManager into the package repository URL text field
    Link KeyboardManager to your application target

GitHub

 
