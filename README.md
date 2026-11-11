# Sign-of-the-Product-of-an-Array
class Solution:
    def arraySign(self, nums: list[int]) -> int:
        if nums is None:
            return 0
        def signFunc(x):
            if x>0:
                return 1
            elif x<0:
                return -1
            else:
                return 0
        product=1
        for i in nums:
            product*=i
        return signFunc(product)
