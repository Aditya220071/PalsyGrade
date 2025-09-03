Bell's Palsy Detection using Machine Learning
This project utilizes machine learning to detect and grade the severity of Bell's Palsy from images and videos.

What is Bell's Palsy?
Bell's Palsy is a neurological condition that causes sudden weakness or paralysis of the muscles on one side of the face. This occurs when the facial nerve, which controls these muscles, becomes inflamed or compressed. While the exact cause is often unknown, it's thought to be associated with viral infections.

Symptoms can appear suddenly and range from mild to severe. They include:

Facial drooping on one side

Difficulty making facial expressions, like smiling or closing an eye

Drooling

Pain around the jaw or behind the ear

Increased sensitivity to sound

The condition is usually temporary, with most people recovering within a few weeks to six months.

Objective
To utilize Machine Learning to grade the severity of Bell's Palsy, which can aid in diagnosis and monitoring recovery.

Approach
Facial Landmark Extraction: We used MediaPipe to extract facial landmarks, precisely masking the mouth region for feature detection.

Dataset and Model: A dataset of over 1000 images was vectorized and used to train a Random Forest model to detect the presence of Bell's Palsy.

Video Evaluation: The model was evaluated on video frames, calculating a severity score as the ratio of affected frames to sampled frames.

Impact
Developed a model with 90% accuracy on images.

Aiming to extend the project for live video-based Bell's Palsy analysis.
