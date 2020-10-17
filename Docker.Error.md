# Error

## unable to fetch daemon.json from the host

再起動で直った。

```
Docker.Core.HttpBadResponseException:
{"status":"error","message":"unable to fetch daemon.json from the host: unable to fetch daemon.json: Get \"http://unix/engine/daemon.json\": context deadline exceeded (Client.Timeout exceeded while awaiting headers)"}

   場所 Docker.Core.Logging.HttpClientExceptionInterceptor.<InterceptResponseAsync>d__0.MoveNext() 場所 C:\workspaces\stable-2.4.x\src\github.com\docker\pinata\win\src\Docker.Core\Logging\HttpClientExceptionInterceptor.cs:行 26
--- 直前に例外がスローされた場所からのスタック トレースの終わり ---
   場所 System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   場所 Docker.Core.Logging.LoggingMessageHandler.<SendAsync>d__4.MoveNext() 場所 C:\workspaces\stable-2.4.x\src\github.com\docker\pinata\win\src\Docker.Core\Logging\LoggingMessageHandler.cs:行 36
--- 直前に例外がスローされた場所からのスタック トレースの終わり ---
   場所 System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   場所 System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   場所 System.Net.Http.HttpClient.<FinishSendAsyncBuffered>d__58.MoveNext()
--- 直前に例外がスローされた場所からのスタック トレースの終わり ---
   場所 System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   場所 System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   場所 Docker.Core.HttpClientExtensions.<GetJsonAsync>d__0`1.MoveNext() 場所 C:\workspaces\stable-2.4.x\src\github.com\docker\pinata\win\src\Docker.Core\HttpClientExtensions.cs:行 16
--- 直前に例外がスローされた場所からのスタック トレースの終わり ---
   場所 System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   場所 System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   場所 Docker.ApiServices.LifecycleClient.<DockerStartAsync>d__10.MoveNext() 場所 C:\workspaces\stable-2.4.x\src\github.com\docker\pinata\win\src\Docker.ApiServices\LifecycleClient.cs:行 122
--- 直前に例外がスローされた場所からのスタック トレースの終わり ---
   場所 System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   場所 System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   場所 Docker.LinuxkitDaemonStartup.<StartAsync>d__5.MoveNext() 場所 C:\workspaces\stable-2.4.x\src\github.com\docker\pinata\win\src\Docker.Desktop\LinuxkitDaemonStartup.cs:行 30
--- 直前に例外がスローされた場所からのスタック トレースの終わり ---
   場所 System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   場所 System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   場所 Docker.Engines.WSL2.LinuxWSL2Engine.<DoStartAsync>d__25.MoveNext() 場所 C:\workspaces\stable-2.4.x\src\github.com\docker\pinata\win\src\Docker.Desktop\Engines\WSL2\LinuxWSL2Engine.cs:行 160
--- 直前に例外がスローされた場所からのスタック トレースの終わり ---
   場所 System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   場所 System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   場所 Docker.ApiServices.StateMachines.TaskExtensions.<WrapAsyncInCancellationException>d__0.MoveNext() 場所 C:\workspaces\stable-2.4.x\src\github.com\docker\pinata\win\src\Docker.ApiServices\StateMachines\TaskExtensions.cs:行 29
--- 直前に例外がスローされた場所からのスタック トレースの終わり ---
   場所 System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   場所 System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   場所 Docker.ApiServices.StateMachines.StartTransition.<DoRunAsync>d__5.MoveNext() 場所 C:\workspaces\stable-2.4.x\src\github.com\docker\pinata\win\src\Docker.ApiServices\StateMachines\StartTransition.cs:行 67
--- 直前に例外がスローされた場所からのスタック トレースの終わり ---
   場所 System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   場所 Docker.ApiServices.StateMachines.StartTransition.<DoRunAsync>d__5.MoveNext() 場所 C:\workspaces\stable-2.4.x\src\github.com\docker\pinata\win\src\Docker.ApiServices\StateMachines\StartTransition.cs:行 92
```
