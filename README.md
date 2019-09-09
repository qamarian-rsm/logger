# Logger

Logger is a Rexa-based Software Main (RbSM), and it records every string sent to it, as
log. When it receives a new string, it prepends the current time to it
(e.g "2019/09/09 23:45:09 "), then sends the string to an io.Writer. The io.Writer decides
where to write the log. The default io.Writer of this RbSM prints logs to the terminal.
To change this behaviour (for instance, if you want your logs to be recorded in a file),
modify the provideWriter () function of this RbSM.

Compatible with Rexa v0.2.0
