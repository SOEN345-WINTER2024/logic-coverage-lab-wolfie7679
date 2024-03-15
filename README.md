Predicate unit test:

public void unit(){
a=true;
b=true;
c=true
assertTrue(checkIt(a,b,c));
assertTrue(checkIt(false,false,false)
}


RACC:

  
  @Test
    public void testPair1() {
        assertTrue(evaluateExpression(true, true, true));  // Decision 1 is true
        assertFalse(evaluateExpression(true, false, true)); // Decision 5 is false
    }

  @Test
    public void testPair2() {
        assertTrue(evaluateExpression(true, true, true));  // Decision 1 is true
        assertFalse(evaluateExpression(false, true, true)); // Decision 6 is false
    }

  @Test
    public void testPair3() {
        assertTrue(evaluateExpression(true, true, true));  // Decision 1 is true
        assertFalse(evaluateExpression(false, false, true)); // Decision 7 is false
    }

  @Test
    public void testPair4() {
        assertTrue(evaluateExpression(true, true, false));  // Decision 2 is true
        assertFalse(evaluateExpression(true, false, true)); // Decision 5 is false
    }

  @Test
    public void testPair5() {
        assertTrue(evaluateExpression(true, true, false));  // Decision 2 is true
        assertFalse(evaluateExpression(false, true, true)); // Decision 6 is false
    }

  @Test
    public void testPair6() {
        assertTrue(evaluateExpression(true, true, false));  // Decision 2 is true
        assertFalse(evaluateExpression(false, false, true)); // Decision 7 is false
    }

  @Test
    public void testPair7() {
        assertTrue(evaluateExpression(true, false, true));  // Decision 3 is true
        assertFalse(evaluateExpression(true, false, true)); // Decision 5 is false
    }

  @Test
    public void testPair8() {
        assertTrue(evaluateExpression(true, false, true));  // Decision 3 is true
        assertFalse(evaluateExpression(false, true, true)); // Decision 6 is false
    }

  @Test
    public void testPair9() {
        assertTrue(evaluateExpression(true, false, true));  // Decision 3 is true
        assertFalse(evaluateExpression(false, false, true)); // Decision 7 is false
    }


    

