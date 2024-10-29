FROM python:3.9

# Set the working directory
# Fixed typo in "appp"
WORKDIR /app  

# Copy the app.py file
# Fixed typo in "appy.py"
COPY app.py /app  

# Install dependencies
# Fixed typo in "netiface"
RUN pip install flask netifaces  

# Expose the port (use numeric values instead of words)
# Changed from "eight thousand" to the actual port number
EXPOSE 8000  

# Set the command to run the application
# Fixed typo in "pythn"
CMD ["python", "app.py"]  
