## Clue
extremely high-performance logger for android

#### Features
- Class name tag(default) or custom tag
- Caller method name
- Source line number information
- Thread name information
- High performance to intercept above information
- Link to source in IDE
- Extensible API

#### Usage
 1. add a log receiver in the application class
    ```java
    public class MyApplication extends Application {
        @Override
        public void onCreate() {
            super.onCreate();
            Clue.addLog(new ConsoleLog()); //init Clue log with default logcat
        }
    }
    ```
 2. call `Clue`'s static methods.

see `sample` application in `clue/sample`




#### License

    Copyright 2017 Clue author

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.