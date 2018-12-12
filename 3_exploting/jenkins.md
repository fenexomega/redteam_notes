# Execute commands on jenkins instance:

def sout = new StringBuffer(), serr = new StringBuffer()
def proc = 'cat /etc/passwd'.execute()
proc.consumeProcessOutput(sout, serr)
proc.waitForOrKill(1000)
println "out> $sout err> $serr"
