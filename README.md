## Tensorflow
Trang chủ, trang đăng ký thi: https://www.tensorflow.org/certificate
Sổ tay về chứng chỉ, những nội dung kiến thức cần thiết tất cả đều có trong: https://www.tensorflow.org/extras/cert/TF_Certificate_Candidate_Handbook.pdf
Hướng dẫn cài đặt môi trường: https://www.tensorflow.org/extras/cert/Setting_Up_TF_Developer_Certificate_Exam.pdf
Link khóa học trên Coursera: https://www.coursera.org/professional-certificates/tensorflow-in-practice
Github các bài code trong khóa học: https://github.com/lmoroney/dlaicourse
 https://github.com/https-deeplearning-ai/tensorflow-1-public

## Dùng hàm Callbacks để kiểm soát đào tạo
 class myCallback(tf.keras.callbacks.Callback):
    def on_epoch_end(self, epoch, logs={}):
        if (log.get('loss') < 0.4):
            print('\n Loss is low so cancelling training!')
            self.model.stop_training = True
 
