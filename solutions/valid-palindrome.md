class Solution:
    def isPalindrome(self, s: str) -> bool:
        left = -1
        right = len(s)
        flag = True

        while left < right :
            right -= 1
            left += 1
            while (left != right) and not (s[right].isalpha() or s[right].isdigit()):
                right -= 1
            while (left != right) and not (s[left].isalpha() or s[left].isdigit()):
                left += 1
            
            if (s[right].isalpha() or s[right].isdigit()) and (s[left].isalpha() or s[left].isdigit()) and (left != right) and (s[right].lower() != s[left].lower()):
                flag = False
                break;
            

        return flag
