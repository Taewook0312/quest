# AIFFEL Campus Online Code Peer Review Templete
- 코더 : 장태욱
- 리뷰어 : 김윤서


# PRT(Peer Review Template)
- [ ]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
      > 파일 내 시각화 되어 있습니다.
    - 문제를 해결하는 완성된 코드란 프로젝트 루브릭 3개 중 2개, 
    퀘스트 문제 요구조건 등을 지칭
      > 루브릭 3조건 모두 충족하셨습니다.
        - 해당 조건을 만족하는 코드를 캡쳐해 근거로 첨부
        ```
        sticker_area = img_bgr[refined_y:refined_y +img_sticker.shape[0],        refined_x:refined_x+img_sticker.shape[1]]
        # img_bgr은 7-2에서 rgb로만 적용해놓은 원본 이미지이다. 
        img_bgr[refined_y:refined_y +img_sticker.shape[0], refined_x:refined_x+img_sticker.shape[1]] = \
        np.where(condition_3d ,sticker_area,img_sticker).astype(np.uint8)
        plt.imshow(cv2.cvtColor(img_bgr, cv2.COLOR_BGR2RGB)) # rgb만 적용해놓은 원본 이미지에 왕관 이미지를 덮어 씌운 이미지가 나오게 된다.
        plt.show()
        ```
- [ ]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
    - 해당 코드 블럭에 doc string/annotation이 달려 있는지 확인
      > 잘 설명되어 있습니다.
    - 해당 코드가 무슨 기능을 하는지, 왜 그렇게 짜여진건지, 작동 메커니즘이 뭔지 기술.
      > 기술되어 있습니다.
    - 주석을 보고 코드 이해가 잘 되었는지 확인
      > LMS의 주석과 동일합니다.
        - 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부합니다.
        
- [ ]  **3. 에러가 난 부분을 디버깅하여 문제를 “해결한 기록을 남겼거나” 
”새로운 시도 또는 추가 실험을 수행”해봤나요?**
    - 문제 원인 및 해결 과정을 잘 기록하였는지 확인
      > 수염 문제를 해결했습니다.
    - 문제에서 요구하는 조건에 더해 추가적으로 수행한 나만의 시도, 
    실험이 기록되어 있는지 확인
      > 잘 처리했습니다.
        - 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부합니다.
          ```
          sticker_area = img_bgr[refined_y:refined_y +img_sticker.shape[0],             refined_x:refined_x+img_sticker.shape[1]]
            # img_bgr은 7-2에서 rgb로만 적용해놓은 원본 이미지이다. 
            img_bgr[refined_y:refined_y +img_sticker.shape[0], refined_x:refined_x+img_sticker.shape[1]] = \
            np.where(condition_3d ,sticker_area,img_sticker).astype(np.uint8)
            plt.imshow(cv2.cvtColor(img_bgr, cv2.COLOR_BGR2RGB)) # rgb만 적용해놓은 원본 이미지에 왕관 이미지를 덮어 씌운 이미지가 나오게 된다.
            plt.show()
          ```
          
        
- [ ]  **4. 회고를 잘 작성했나요?**
    - 주어진 문제를 해결하는 완성된 코드 내지 프로젝트 결과물에 대해
    배운점과 아쉬운점, 느낀점 등이 기록되어 있는지 확인
    - 전체 코드 실행 플로우를 그래프로 그려서 이해를 돕고 있는지 확인
        - 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부합니다.
        > 회고 잘썼습니다.
        
- [ ]  **5. 코드가 간결하고 효율적인가요?**
    - 파이썬 스타일 가이드 (PEP8) 를 준수하였는지 확인
    - 하드코딩을 하지않고 함수화, 모듈화가 가능한 부분은 함수를 만들거나 클래스로 짰는지
    - 코드 중복을 최소화하고 범용적으로 사용할 수 있도록 함수화했는지
        - 잘 작성되었다고 생각되는 부분을 캡쳐해 근거로 첨부합니다.
      > 주석이 투 머치한 느낌이 들지만, 설명을 도와주어서 좋았습니다. 전반적으로 모든 코드가 잘 작성되었습니다. 


# 참고 링크 및 코드 개선
```
# 코드 리뷰 시 참고한 링크가 있다면 링크와 간략한 설명을 첨부합니다.
# 코드 리뷰를 통해 개선한 코드가 있다면 코드와 간략한 설명을 첨부합니다.
```
