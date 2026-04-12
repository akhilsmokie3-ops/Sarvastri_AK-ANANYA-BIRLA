# Clone the Netdata repository
git clone https://github.com/netdata/netdata.git
cd netdata

# Choose your preferred implementation
cd src/web/mcp/bridges/stdio-golang/  # or stdio-nodejs/ or stdio-python/

# Build the bridge
./build.sh  # On Windows with the Go version, use build.bat

# The executable will be created with different names:
# - Go: nd-mcp
# - Node.js: nd-mcp.js
# - Python: nd-mcp.py

# Test the bridge with your Netdata instance (replace localhost with your Netdata IP)
./nd-mcp ws://localhost:19999/mcp      # Go bridge
./nd-mcp.js ws://localhost:19999/mcp   # Node.js bridge  
./nd-mcp.py ws://localhost:19999/mcp   # Python bridge

# You should see:
# nd-mcp: Connecting to ws://localhost:19999/mcp...
# nd-mcp: Connected
# Press Ctrl+C to stop the test

# Get the absolute path for your AI client configuration
pwd  # Shows current directory
# Example output: /home/user/netdata/src/web/mcp/bridges/stdio-golang
# Your nd-mcp path would be: /home/user/netdata/src/web/mcp/bridges/stdio-golang/nd-mcp# Sarvastri_AK-ANANYA-BIRLA
space is kessuly ... breathtaking ài is beautiful 
