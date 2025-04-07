from flask import Flask, request, jsonify
import os

app = Flask(__name__)

# Set the upload folder and allowed file extensions
UPLOAD_FOLDER = 'uploads'
ALLOWED_EXTENSIONS = {'sb3'}

app.config['UPLOAD_FOLDER'] = UPLOAD_FOLDER

# Function to check allowed file extensions
def allowed_file(filename):
    return '.' in filename and filename.rsplit('.', 1)[1].lower() in ALLOWED_EXTENSIONS

@app.route('/submit_quiz', methods=['POST'])
def submit_quiz():
    if 'projectFile' not in request.files:
        return jsonify({'error': 'No file part'}), 400
    file = request.files['projectFile']

    if file.filename == '':
        return jsonify({'error': 'No selected file'}), 400

    if file and allowed_file(file.filename):
        filename = os.path.join(app.config['UPLOAD_FOLDER'], file.filename)
        file.save(filename)

        # Assume you calculate the score here based on project file submission
        score = 8  # Just an example, you can calculate the score based on project content

        return jsonify({'message': 'File successfully uploaded', 'score': score})
    else:
        return jsonify({'error': 'Invalid file format'}), 400

if __name__ == '__main__':
    app.run(debug=True)
